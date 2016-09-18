https://repl.it/DcTo/0


```javascript
    // makes a person for the chatroom
    var Participant = function(name) {
        this.name = name;
        this.chatroom = null;
    };
     
    Participant.prototype = {
        send: function(message, to) {
            this.chatroom.send(message, this, to);
        },
        receive: function(message, from) {
            log.add(from.name + " to " + this.name + ": " + message);
        }
    };
     // makes a chatroom
    var Chatroom = function() {
        var participants = {};
     
        return {
     
            register: function(participant) {
                participants[participant.name] = participant;
                participant.chatroom = this;
            },
     
            send: function(message, from, to) {
                if (to) {                      // single message
                    to.receive(message, from);    
                } else {                       // broadcast message
                    for (key in participants) {   
                        if (participants[key] !== from) {
                            participants[key].receive(message, from);
                        }
                    }
                }
            }
        };
    };
     
    // log helper
     
    var log = (function() {
        var log = "";
     
        return {
            add: function(msg) { log += msg + "\n"; },
            show: function() { alert(log); log = ""; }
        }
    })();
     
    function run() {
        var bob = new Participant("Bob");
        var doug = new Participant("Doug");

        var chatroom = new Chatroom();
        chatroom.register(bob);
        chatroom.register(doug);

        doug.send("hey guys.");
        bob.send("hey doug",doug);
     
        log.show();
    }
```
