__Model:__<br />
predicts that a customer will buy again from the audio book company so that it will not spend its advertisement budget on individuals who are unlikely to come back.
This is a classification problem with two classes: won't buy and will buy, represented by 0s and 1s.<br />

__Technology:__<br />
Neural Network with Tensorflow.<br />


__The database:__<br />
There are several variables: <br />
Customer ID, <br />
Book length overall (sum of the minute length of all purchases), <br />
Book length avg (average length in minutes of all purchases), <br />
Price paid_overall (sum of all purchases),<br />
Price Paid avg (average of all purchases), <br />
Review (a Boolean variable whether the customer left a review), <br />
Review out of 10 (if the customer left a review,8.91 is the average so we don't left it empty., <br />
Total minutes listened,<br />
Completion (from 0 to 1), minutes listened / book length overall,<br />
Support requests (number of support requests; everything from forgotten password to assistance for using the App), Last visited minus purchase date (in days).<br />
<br />
These are the inputs (excluding customer ID, as it is completely arbitrary. It's more like a name, than a number).<br />
<br />
The targets are a Boolean variable (0 or 1). <br />
We are taking a period of 2 years in our inputs, and the next 6 months as targets. So, in fact, we are predicting if: based on the last 2 years of activity and engagement, a customer will convert in the next 6 months. 6 months sounds like a reasonable time. If they don't convert after 6 months, chances are they've gone to a competitor or didn't like the Audiobook way of digesting information.<br />

