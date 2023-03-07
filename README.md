# int20h_23_tt
## Hackathon INT20H test task
Team KryMor:
- Oleg Morhaliuk
- Maksym Kryvenko

## Data Set Description 
This data set represents the behavioral data of a utility app designed for car-related 
transactional services. The app is subscription-based, and users are charged monthly or 
annually.
The transaction (event «Transaction») is the primary feature that proves the user is getting value 
from the product. As long as the user has them - there is an economic sense for this user to 
keep paying for the app.
App operates in various regions of the United States, and the service structure differs 
significantly from state to state as the service/transaction availability differs for each state.
Also, users have slight differences, some of them need to conduct transactions more 
frequently, and some less often. The best example, in this case, would be Uber - some people 
need to drive more regularly, and some use the app only occasionally.
The dataset contains data for the year 2022 and has the next events:
- Transaction Refund - user receives a refund, because he probably didn’t perform the 
Transaction and was charged by mistake
- Order - target transaction performed, also has multiple event properties included
- Account Setup Skip - users skip registration
- Signup Success - successful registration, includes information about the Signup method - 
social network, email, etc
- Add Vehicle Success - vehicle registration, part of the onboarding process, also includes the 
information about the vehicle.
- Add Vehicle Break - user didn’t complete vehicle registration
- Add Payment Method Sucess - user adds the credit card
- Add Payment Method Failed - user experiences failure while adding the payment method
- Email Confirmation Success - user passes through the email verification process, now we are 
user he receives messaging from the product
- Chat conversation Opened - user contacts the Support, that’s usually is not good, something 
is probably going wrong
- Sign Out - user signs out from the account, maybe he even wants to terminate the 
subscription, but this is not a complete action to close the account
- Account History Transaction Details - user checks some particular transactions, usually he is 
either savvy and likes to audit the expenses or he has a suspicion that there might be some 
billing errors
- Wallet Opened - user checks his balance state
- Subscription Premium - user buys a monthly or annual subscription
- Subscription Premium Cancel - explicit churn event - user has canceled the subscription. 
That’s the event we want to predict and prevent
- Calculator view - users want to get an idea about the cost of future transaction

## Assignment 
Identify a set of events and parameters with the highest or lowest correlation with the potential 
account cancellation. Prioritize the events, event properties or user properties, which have 
highest or lowest correlation with the account cancellation
