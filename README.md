# FundOfProg



PROBLEM STATEMENT:
  A program is required that asks a loan applicant to enter his / her credit score and the 
  program will decide whether the applicant is qualified for a loan or not based on the min  
  660 score requirement for the CVTC bank located in Eau Claire, WI. Then, for non-qualified 
  applicants, it will output and display the qualification results. If the applicant is 
  eligible, the will set a right interest rate for the credit score and ask the applicant to  
  enter a home value, downpayment percentage, loan start-year, and month. It will convert 1-12
  month input to a month name. Then, it will calculate the total downpayment, loan amount, 
  start date (mm, yyyy), payoff date, total cost of loan, monthly principal & interest, monthly 
  property tax, and monthly homeowner’s insurance for a 10, 15, 20, 25 and a 30-year loan term. 
  Finally, it will display all the calculated results including the prompted inputs.

  NOTE: Set variable the interest rate at 7.63% if credit score is between 660 and 679
                                       at 7.13% if credit score is between 679 and 699
                                       at 6.99% if credit score is between 699 and 719
                                       at 6.87% if credit score is between 719 and 739
                                   and at 6.75% if credit score is 739 and above.
        Also, given property tax rate is 8.55% and the home insurance is estimated near the 1.88% of monthly loan payment. 

NOUNS:
  Credit score, min 660-score, interest rate, home value, downpayment percentage, loan start-year 
  & month, total down-payment, loan amount, start date (mm, yyyy), payoff date, total cost of loan,
  monthly principal & interest, monthly property tax, monthly homeowner’s insurance, 10, 15, 20, 25
  and 30-year terms.

VERBS:
  Ask, decide, set, output, display, calculate




DEFINING DIAGRAM:

INPUTS
  credit score
  home value
  downpayment percentage
  loan start-year
  loan start-month

PROCESSING:
  prompt a user for a credit score
  output a message for a non-qualified user 
  assign the right interest rate for the qualified user 
  prompt a qualified user for more inputs: home value downpayment percentage loan start-year loan start-month
  convert a month number to a month name
  output a start-date
  output a payoff date
  calculate the cost of a loan
  calculate the downpayment amount
  calculate the loan amount
  calculate the monthly principal & interest
  calculate the monthly property tax
  calculate the monthly home insurance
  calculate the total loan monthly payment

OUTPUTS:
  message for a not-qualified user
  credit score
  home value
  start date
  End-date
  down-payment amount 
  loan amount
  cost of a loan
  Monthly principal & interest
  Monthly property tax
  monthly home insurance
  total monthly loan payment




PSEUDOCODE (SOLUTION ALGORITM):

calculateTotalMonthlyLoanPayment
  prompt a user for a credit score
    IF credit score is smaller than 660 THEN 
      Output a message - you're not a qualified for a loan
    ELSE
      IF credit score is >= 660 and <= 679 THEN
        Set interest rate at 7.63%
      ELSEIF credit score is > 679 and <= 699 THEN
        Set interest rate at 7.13%
      ELSEIF credit score is > 699 and <= 719 THEN
        Set interest rate at 6.99%
      ELSEIF credit score is > 719 and <= 739 THEN
        Set interest rate at 6.87% 
      ENDIF 
        Set interest rate at 6.75%
    Prompt a user for the home value
    Prompt a user for the downpayment percentage
    Prompt a user for the loan start-year
    Prompt a user for the loan start-month
    Convert home value downpayment to numbers
      SWITCH start-month
         CASE "1": THEN
           Assign "Jan"
         CASE "2": THEN
           Assign "Feb"
         CASE "3": THEN
           Assign "Mar"
         CASE "4": THEN
           Assign "Apr"
         CASE "5": THEN
           Assign "May"
         CASE "6": THEN
           Assign "Jun"
         CASE "7": THEN
           Assign "Jul"
         CASE "8": THEN
           Assign "Aug"
         CASE "9": THEN
           Assign "Sep"
         CASE "10": THEN
           Assign "Oct"
         CASE "11": THEN
           Assign "Nov"
         CASE "12": THEN
           Assign "Dec"
      ENDCASE
         Output msg Invalid number
    Output startdate
      Calculate the total downpayment
      Calculate the loan amount
      Calculate the monthly interest
      Display home value
      Display credit score 
      Display total downpayment
      Display loan amount
      Display interest rate
      Display start-date
    FOR loop runs for 10, 15, 20, 25 and 30 loan-terms
      Convert annual loan term to monthly
      Calculate monthly loan payment
      Calculate total cost of the loan
      Calculate monthly property tax
      Calculate monthly home insurance
      Calculate the pay off year
      Output payoff date
      Display monthly loan payment
      Display total cost of the loan
      Display monthly property tax
      Display monthly home insurance
      Display the pay off year
      Display payoff date
  ENDIF
END

      
 
      
  


