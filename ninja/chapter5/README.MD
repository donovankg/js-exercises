1. Implement the following: 
  1. A bank that holds client’s information: 
    1. account number; 
    2. balance 
  2. A set of clients where each can: 
    1. hold money of their own; 
    2. deposit money into the bank (to any account); 
    3. retrieve money from the bank (from personal account only); 
    4. view current balance in bank (from personal account only) 
  3. A client cannot deposit more money than what it has; 
  4. A client cannot retrieve more money that what is in its account; 
  5. All financial information must be private 
  
  Use of closures  

```javascript
//Exercise 1
//Outer function
var bankInstance = new Bank("mybank");
var acc = bankInstance.createAccount("long",1,"hi");
acc.getNumber("hi");
var anishacct = bankInstance.createAccount("Anish", 100000,"gohome");
anishacct.getNumber("gohome");
//Inner funtion
function Bank(name){
	
	var accounts={};
	var id=1;
	this.name=name;
	this.createAccount=function account(name, balance,key) {
		var accId=id++;
		accounts[accId]={
			name:name,
			amount:balance
		};
	return {
		getNumber: function (key1) {
			if(key==key1)
			return { 
				name: accounts[accId].name,
				amount: accounts[accId].amount
			};
				
		},
		
//balance
		getBalance: function(key1) {
			if(key==key1)
			return accounts[accId].balance;
		
		},
//deposit
		deposit: function(money) {
			balance += money;
			return balance;
		},
//deposit		
		withdraw: function(cash) {
			if (balance > cash){
				balance -= cash;
				return balance;
			}
		
		return "Insufficient funds";
		
		}
	};

};
}


```



2. Implement the following: 
  
  A large building has many people and pieces of equipment. A new tech­support employee has been hired to help out solve users’ problems and fix broken 
  equipment. The new employee is still unfamiliar with the layout but is doing his best to keep track of where everyone and everything is. 
    1. Implement a structure that represents the building. 
    2. Must contain data types representing equipment and users. ii. Equipment can be associated with rooms or specific people 
    3. Each piece of equipment and person is associated with a specific floor and room. 
    4. The new tech­support employee must be able to find users and equipment as quickly as possible. 

  Use of memoization and implementation of a simple searching algorithm. 
