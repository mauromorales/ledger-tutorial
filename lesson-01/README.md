# Lesson 01: Opening Balances & Net Worth

## Opening Balances

> In order to keep track of your finances you need to start somewhere or better
> yet, some time. Opening balances is a reference to the money you have (Assets)
> and owe (Liabilities) at a given moment in time.

Last year Helmut had a hard time saving money for his dream vacation. Lots of
that money went into late payments of his credit card. He's always anxious
because he never knows how much he's spend each month on new apps for his phone.

His 2015 resolution was to hack for once and for all his finances so he went
online and found Ledger CLI. He installed it and logged into GeekBank's website
to see how much money he had. He has one checkings account with $900 and
a MasterCard where he currently owes $75.

He put the information into a journal.dat file and it looked like this:

```
2015/01/01 Opening Balances
  Assets:GeekBank:Checking               $900.00
  Liabilities:GeekBank:Mastercard        $-75.00
  Equity:Opening Balances
```

## Net Worth

> Your net worth is a snapshot of your financial situation in a specific point
> in time. It is very important because it will tell you how healthy your
> finances are. You should run this report periodically (i.e.: monthly) so you
> can measure if you are getting better or worse.
>
> Now when you buy something you will be able to make an informed decision. And
> if you have plans in the future like a dream vacation or saving for your car,
> you can determine your starting point.

Helmut wants to see what is his net worth so he can determine how he started the
year. He runs in the command line:

```
ledger -f journal.dat balance Assets Liabilities
```

And Ledger gives him back the following output:

```
             $900.00  Assets:GeekBank:Checking
             $-75.00  Liabilities:GeekBank:Mastercard
--------------------
             $825.00
```

Helmut started the year with a net worth of $825. He is exited that it only took
about fife minutes of his time. He is excited to see how things develop next
week in lesson 02 when he starts putting in his income and expenses.
