A = load 'Transactions.csv' using PigStorage (',');
B = load 'MoreTransactions.csv' using PigStorage (',');
C = union A,B;
D = group C by 1;
E = foreach D generate flatten (C);
store E into 'Results';
