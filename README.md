# Banking-Application-Project
We want to create a Banking Software with functions like
1.	Deposit
2.	Withdraw
3.	Show Balance

In fact, having data and performing certain operation on that data is very basic characteristic in any software program.
Therefore, the birth of Object Oriented Programming which is commonly called OOPS.
The same code in Object Oriented Programming languages will have same data and some action performed on that data.
By combining data and action, we will get many advantages over structural programming viz,
•	Abstraction
•	Encapsulation
•	Inheritance
•	Polymorphism
•	
•	We will discuss how it has been used in our coding part ‘
•	First we will see Abstraction Concept :-
•	Abstraction is the concept of object-oriented programming that “shows” only essential attributes and “hides” unnecessary information. The main purpose of abstraction is hiding the unnecessary details from the users. Abstraction is selecting data from a larger pool to show only relevant details of the object to the user. It helps in reducing programming complexity and efforts. It is one of the most important concepts of OOPs.
•	we want to create a banking application and we are asked to collect all the information about our customer. There are chances that we will come up with following information about the customer
•	But, not all of the above information is required to create a banking application.
•	So, we need to select only the useful information for our banking application from that pool. Data like name, address, tax information, etc. make sense for a banking application which is an Abstraction example in OOPs
•	Since we have fetched/removed/selected the customer information from a larger pool, the process is referred as Abstraction in OOPs.
•	However, the same information once extracted can be used for a wide range of applications. For instance, we can use the same data for hospital application, job portal application, a Government database, etc. with little or no modification. Hence, it becomes our Master Data. This is an advantage of Abstraction in OOPs.
•	In OUR PROGRAMMING PART SAME CONCEPT WE HAVE USED … we are only dealing with Account No,Account type, Account Holder’s Name etc..which is relevant information.. 
Now We will see how Encapsulation Concept is used in our programming part 
First of all 
What is Encapsulation in Java?
Encapsulation in Java is a mechanism to wrap up variables (data) and methods(code) together as a single unit. It is the process of hiding information details and protecting data and behaviour of the object. It is one of the four important OOP concepts. The encapsulate class is easy to test, so it is also better for unit testing.

To understand what is encapsulation in detail consider the following bank account class with deposit and show Account methods which have written in the Notepad
Suppose a hacker managed to gain access to the code of our bank account. Now, he tries to deposit amount -100 into our account
He tries to deposit an invalid amount (say -100) into our bank account by manipulating the code.
If a data member is private, it means it can only be accessed within the same class. No outside class can access private data member or variable of other class.
So in our case hacker cannot deposit amount -100 to customer’s account.
The entire code can be thought of a capsule, and we can only communicate through the messages. Hence the name encapsulation.
We will see now Inheritance Concept which is used here
First of all What is Inheritance?
Inheritance is a mechanism in which one class acquires the property of another class. For example, a child inherits the traits of his/her parents. With inheritance, we can reuse the fields and methods of the existing class. Hence, inheritance facilitates Reusability and is an important concept of OOPs.
For Example As you can see in the Diagram Class B extends only Class A. Class A is a super class and Class B is a Sub-class
Similarly in our programming part 
 Here I have Written class BankingApplication extends BankDetails means BankingApplication inherited traits from their parent Class BankDetails so it is the example of Single Inheritance 
In the Notepad We can see How BankingApplication inherited traits from their parent Class BankDetails so it is the example of Single Inheritance. 
So it Will retrieve all the information   which I have already coded like., Account NO, Account  holder name etc. coded from parent class BankDetails

Now We will see How Polymorphism can be used in our Bank Management System But First of all it is necessary to know..
What is Polymorphism in Java?
Polymorphism in Java occurs when there are one or more classes or objects related to each other by inheritance. It is the ability of an object to take many forms. Inheritance lets users inherit attributes and methods, and polymorphism uses these methods to perform different tasks. So, the goal is communication, but the approach is different.
In the coding part 
We have one parent class, ‘Account’ with function of deposit and withdraw. Account has 2 child classes
The operation of deposit and withdraw is same for Saving and Checking accounts. So the inherited methods from Account class will work.
There is a change in the requirement specification, something that is so common in the software industry. we are supposed to add functionality privileged Banking Account with Overdraft Facility.
For a background, overdraft is a facility where you can withdraw an amount more than available the balance in your account.
So, withdraw method for privileged needs to implement afresh. But you do not change the tested piece of code in Savings and Checking account. This is advantage of OOPS
As You all can see in the Diagram:-
In the Step 1) Such that when the “withdrawn” method for saving account is called a method from parent account class is executed

Step 2) is that  when the “Withdraw” method for the privileged account (overdraft facility) is called withdraw method defined in the privileged class is executed. This is Polymorphism in OOPs. 
   public void openAccount() is used here to take details from Customer’s like Account No and depositing money and creating a n 
Deposit money function is created to deposit money to the account by asking amount by the customer. 
It will ask the amount and add it to the available balance. 
Where
Display Account function will show the details of the customer like name, address, type of account and available balance. Total Balance = Available Balance + Deposited Amount
Withdraw money function is created to withdraw money from the account by asking amount by the customer. 
It will ask the amount and subtract it from the available balance. 
Total Balance = Available Balance – Withdrawal Amount


