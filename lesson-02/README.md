# Lesson 02: Income and Expenses & Cash Flow

## Income and Expenses

> Every time we spend money or give it away for a cause we make an expense. You
> want to categorize your expenses so that you can determine where your money is
> going easily.
>
> When you get paid or money is gifted to, you have an income.

January is almost over. Helmut has been diligent about putting his expenses
every week. He decided to take a few minutes every Sunday night to keep track of
his finances, so he can start the week without any worries. I've added some
comments to his transactions so you can get some context.

Helmut decided he was not going to pay any late fee on his credit card so he
went online and did a transfer from his Checkings account to his MasterCard.

In order to make his life easier Helmut will only keep records of his expenses
online. There is always the need for cash but it's minimal and he thinks he can
treat it as a miscellaneous and not worry about the details.

```
2015/01/01 Linode
  ;Personal production server and development server
  Expenses:Services and Equipment         $80.00
  Liabilities:GeekBank:Mastercard

2015/01/02 Lanlord Inc.
  ;Nice apartment in city center
  Expenses:Rent                         $1100.00
  Liabilities:GeekBank:Mastercard

2015/01/02 StarBucks
  ;<3 Coffee
  Expenses:Coffee                          $3.65
  Liabilities:GeekBank:Mastercard

2015/01/03 InterTelco
  ;Home internet & mobile
  Expenses:Services and Equipment        $120.00
  Liabilities:GeekBank:Mastercard

2015/01/04 The Lobster
  Expenses:Dining Out                     $44.00
  Liabilities:GeekBank:Mastercard

2015/01/05 Wallmart
  Expenses:Groceries                     $320.32
  Liabilities:GeekBank:Mastercard

2015/01/07 StarBucks
  Expenses:Coffee                          $3.65
  Liabilities:GeekBank:Mastercard

2015/01/12 Amazon.com
  Expenses:Books                          $73.20
  Expenses:Gadgets                       $249.00
  Liabilities:GeekBank:Mastercard

2015/01/13 StarBucks
  Expenses:Coffee                          $3.65
  Liabilities:GeekBank:Mastercard

2015/01/14 Netflix
  Expenses:Subscriptions                   $7.99
  Liabilities:GeekBank:Mastercard

2015/01/15 Mario's Trattoria
  Expenses:Dining Out                     $23.00
  Liabilities:GeekBank:Mastercard

2015/01/17 Cash
  Expenses:Cash                          $100.00
  Liabilities:GeekBank:Mastercard

2015/01/18 DevelopmentCasts
  Expenses:Subscriptions                   $9.00
  Liabilities:GeekBank:Mastercard

2015/01/18 The Bar
  Expenses:Drinks                         $39.00
  Liabilities:GeekBank:Mastercard

2015/01/19 StarBucks
  Expenses:Coffee                          $3.65
  Liabilities:GeekBank:Mastercard

2015/01/20 GeekBank
  ; pay last month in full
  Liabilities:GeekBank:Mastercard         $75.00
  Assets:GeekBank:Checking

2015/01/20 Tablet Magazine
  Expenses:Subscriptions                  $14.00
  Liabilities:GeekBank:Mastercard

2015/01/21 Google Play Store
  Expenses:Apps & Games                    $2.00
  Liabilities:GeekBank:Mastercard

2015/01/22 CityTransport
  ; monthly card
  Expenses:Transport                      $65.00
  Liabilities:GeekBank:Mastercard

2015/01/27 Hard Rock Cafe
  Expenses:Dining Out                     $45.00
  Liabilities:GeekBank:Mastercard

2015/01/28 Gifts and Co.
  ; Sandra's birthday
  Expenses:Gifts                          $30.00
  Liabilities:GeekBank:Mastercard
```

Helmut works as a junior web developer for a company called CodingChamaleons.
They make a deposit in his account the last week of the month.

```
2015/01/26 CodingChamaleons
  Assets:GeekBank:Checking              $3500.00
  Income:Salary
```

He runs his net worth report in order to see where he stands.

```
            $3325.00  Assets:GeekBank:Checking
           $-2336.11  Liabilities:GeekBank:Mastercard
--------------------
             $988.89
```

It increased which is really good news, but not by much. Let's see what happened
here.

## Cash Flow

> Your Cash Flow is the difference between your income and expenses. If you are
> earning less than what you spend, you are in big trouble and this is not
> sustainable. On the other hand if you manage to save money every month you are
> on the right track.

```
ledger -f journal.dat balance Income Expenses
```

And Ledger gives him back the following output:

```
            $2336.11  Expenses
               $2.00    Apps & Games
              $73.20    Books
             $100.00    Cash
              $14.60    Coffee
             $112.00    Dining Out
              $39.00    Drinks
             $249.00    Gadgets
              $30.00    Gifts
             $320.32    Groceries
            $1100.00    Rent
             $200.00    Services and Equipment
              $30.99    Subscriptions
              $65.00    Transport
           $-2500.00  Income:Salary
--------------------
            $-163.89
```

Helmut's cash flow for January was -$163.89. Because of how we treat income and
expenses negative is good. It means he saved $163.89 this month but if he
expects to save enough for his dream vacation this will take forever. He needs
to analyze his expenses and cut some expenses.


