# HW4 - Implementation & Debugging

Hi there! Welcome to Yujin and Yuqi's Expense Tracker App! This README.md file is inherited from HW3.


# New Functionalities

## Model

The Observer Design Pattern is applied for this homework. In model package, new functions below were added:
public boolean register(ExpenseTrackerModelListener listener){};
public boolean unregister(ExpenseTrackerModelListener listener){};
public int numberOfListeners(){};
public boolean containsListener(ExpenseTrackerModelListener listener){};
protected void stateChanged(){};

## Controller

In the controller package, view.update(model) was commented out.


## Compile

To compile the code from terminal, use the following command:
```
cd src
javac ExpenseTrackerApp.java
java ExpenseTrackerApp
```

You should be able to view the GUI of the project upon successful compilation. 


## How to use

After the application is compiled, you will see a panel with input fields and buttons. 

On the top, you can enter the amounts and categories of your transactions, click "Add Transaction" button to add your transaction to current central panel. If you find yourself enter something run and want to revoke the transaction, feel free to click "Undo" button to cancel your addition. **You can also delete many transactions together in one time!**

If you want to know what transaction do you have between a certain amount, or what transaction do you have with a certain category, you can use "Filter by amount" button and "Filter by category" button. Transactions that fulfill the conditions will be highlighted in light green.

Hope you have a great time playing with this application!


## Testing

All test cases are passed as shown in the screenshots PDF file.


## Java Version
This code is compiled with ```openjdk 17.0.7 2023-04-18```. Please update your JDK accordingly if you face any incompatibility issue.