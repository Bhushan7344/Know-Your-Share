# Know-Your-Share
Know Your Share is an application which can be used to split bills among a group of people.
Know your Share is a program that allows a group of users to keep track of their
informal debts like travel expenses, bills, and rentals. A group of users enters the data
into the app about whom they owe, who owes them, and why. This comes very handy
in cases where a group of friends or a family decides to go to a restaurant or a trip. All
the costs and the bills need to be kept track of. The debts are read as a directed graph
and the cash flow is minimized using the Greedy algorithm. The directed graph is
converted into a cost adjacency matrix and given as a parameter. The output of the
program gives the minimum payment to be made by each of the users in order to solve
all the debts. This service eliminates the need to keep receipts because a user can add
an expense whenever the cost is incurred. This can avoid many confusions regarding
the payments and can lead to many misunderstandings. A detailed report of the debt
settlement is given as the output. This report is generated and stored in a file and
hence can be stored permanently. In this way, we can reduce unnecessary transactions
or confusion regarding debts.

Algorithm
The detailed algorithm of the minimum cash flow algorithm is given below Do following for every person Pi where i is from 0 to n-1. 
1. Compute the net amount for every person. The net amount for person ‘i’ can be computed by subtracting sum of all debts from sum of all credits. 
2. Find the two persons that are maximum creditor and maximum debtor to the person Pi. 
3. Let the maximum amount to be credited maximum creditor be maxCredit and maximum amount to be debited from maximum debtor be maxDebit. 
4. Let the maximum debtor be Pd and maximum creditor be Pc. 
5. Find the minimum of maxDebit and maxCredit. 
6. Let minimum of two be x. 
7. Debit ‘x’ from Pd and credit this amount to Pc 
8. If x is equal to maxCredit, then remove Pc from set of persons and recur for remaining (n-1) persons. 
9. If x is equal to maxDebit, then remove Pd from set of persons and recur for remaining (n-1) persons.
