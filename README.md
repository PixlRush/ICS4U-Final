# ICS4U1-E1 Final Project
## Proposal
I would like to make a command-line banking service. It will be able to store and print multiple accounts per user, have a username and password (hashed in storage) for each user, be able to deposit and withdraw funds with throwing the correct exceptions whenever needed.
## UML
### User
Commandable >>
```
Account[] accounts
String name
String password
```
```
boolean login()
getBalances()
toString()
```
### Account
Commandable >>
```
double value
Ledger ledger
```
```
deposit()
withdraw()
transfer()
```
### Ledger
```
ArrayList<Modification> changes
```
```
toString()
getTransaction(Date)
```
### Modification
```
Date time
double value
```
```
toString()
getTime()
getValue()
```
### Commandable
```
cmd(String[])
```
## Test Cases
