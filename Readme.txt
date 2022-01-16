README FILE - AKSHAY MEDIRATTA 1130041

GENERAL PROBLEM - This assignment helps us in managing the stocks and mutual funds inventory for a person.
		  Here, we have implemented Graphic user Interface to make the process better.
                  There are 5 files that I made, Stock, Mutualfund, ePortfolio, investment, Assignment3GUI
 
ASSUMPTIONS     - All basic assumptions requiered for the assignment.
		  It is assumed that the user would first put in an entry and then use the other options.
                     
LIMITATIONS -     As per my understanding, there are no limitations to my program (as per assignment description)    

STEPS TO COMPILE - Once you are in the folder amedirat_a3, type the statement
		   javac ePortfolio/*.java
		   followed by the statement
		   java ePortfolio.Assignment3GUI    
  
1)  The problem of reusing the code again and again or the redudancy of code was solved using an extend statement 
   followed by an @override command to avoid duplicacy of code and unneccesary wastage of time. 

2) TEST PLAN 
   I thoroughly tested the entire code with several challenging inputs and made sure nothing went wrong.

   For example, if we initially buy 500 shares of AAPL stock at the price of $110.08 per share, the quantity will be 500, 
   and the bookValue will be 500 × 110.08 + 9.99 = $55,049.99. Later on, if the price is changed to $142.23 per share, 
   the gain will be (500 × 142.23 – 9.99) – 55,049.99 = 71,105.01 – 55,049.99 = $16,055.02. 
   Alternatively, if we sell 200 shares of this stock at $142.23 per share, the payment received will be 200 × 142.23 – 9.99 = $28,436.01, 
   the quantity will be reduced to 300, and bookValue will be adjusted to 55,049.99 × 300/500 = $33,029.99.

   For each mutual fund, we do not pay any fee if we buy certain units of the fund, but if we sell certain units of the fund, 
   we need to pay a redemption fee of $45. For instance, if we initially buy 450 units of SSETX at $53.26 per unit, 
   the quantity will be 450 and the bookValue will be 450 × 53.26 = $23,967.00. Later on, if the price goes down to $42.21 per unit, 
   the gain will be (450 × 42.21 – 45.00) – 23,967.00 = 18,949.50 – 23,967.00 = –$5,017.50. 
   Alternatively, if we sell 150 units of this fund at $42.21 per unit, the payment received will be 150 × 42.21 – 45.00 =
   $6,286.50, the quantity will be reduced to 300, and the bookValue will be changed to 23,967.00×300/450 = $15,978.00.
   
   I catered several cases like:-
   => In sell function, if user enters a symbol which doesn’t exist, “No investment found” is displayed.   
   => In search function too, if the user enters some wrong inputs, no match found is displayed.
   => While purchasing some investment, I made sure that symbols don’t overlap.

5) Possible improvements
   I can make my search function work better and in an efficient way.