# termbank

Bank like it's 1980. View bank account details and statements in the terminal.

For Lloyds bank customers only. Essentially a reverse engineer of their login protocol with some messy screen-scraping.

## Usage

Assuming your `$PATH` contains `$GOPATH/bin` then download and compile with:

```bash
$ go get github.com/st3redstripe/termbank
``` 

Execute `termbank` and follow the instructions.

Typical program run:

```bash
$ termbank
User ID: *******
Password: *******
Memorable Info: *******

Logged in!

1) Account 1 - £xxxx.xx
2) Account 2 - £xxxx.xx
3) Account 3 - £xxxx.xx

Enter valid account number: 1

Account: Account 1
Balance: £xxxx.xx
Fetching statement...

Transaction  Sort Code  Account Numb  Transaction   Debit Amount  Balance
30/10/2013   99-99-99   12345678      TESCO STORES  5.15          1006.64
29/10/2013   99-99-99   12345678      TESCO STORES  5.63          1011.79
...
```
