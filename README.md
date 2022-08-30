# Diamond-Price-Prediction

In this project I want to predict Diamond Prices based on Cut, Color, Clurity and other attributes. I have chosen the simple structure diamonds dataset from the Kaggle website.

----

<ins>DataSet:</ins>

The dataset consists of 53,940 entries of diamonds and contains 11 columns (10 of them are features and 1 is the target value.)

<ins>Main features:</ins>

<p>&#8900; Index counter (Specific index of record) </p>
              
<p>&#8900; carat   (Weight of the diamond)</p>

<p>&#8900; cut     (Quality of the diamond, which onsists of fair, good,very good,premium,ideal)</p>
              
<p>&#8900; color   (Color of the diamond)</p>
              
<p>&#8900; clarity (How clear the diamond is)</p>
              
<p>&#8900; price   (Price of the diamond)</p>
               
<p>&#8900; table   (width of top of diamond relative to widest point)</p>
              
<p>&#8900; x       (Length in mm)</p>
            
<p>&#8900; y       (Width in mm)</p>
               
<p>&#8900; z       (depth in mm)</p>
               
<p>&#8900; depth   (total depth percentage = z / mean(x, y))</p>

----

<p>&#8883; The dataset does not include any missing values. However diamonds with x, y ,z=0 or x, y, z >10 are outliers.</p>

<p>&#8883; The dataset includes 3 categorical variable(cut, color and clarity). I used OrdinalEncoder to encode these categorical vairables.</p>

<p>&#8883; I created a new feature called "volume", which is the multiplication of x, y and z. I removed the x, y, z columns and added a this new "volume" column to the dataset.</p>

<p>&#8883; I split the dataset into train and test set. I used tree different models (Linear Regression, Decision Tree Regressor and Random Forest Regressor) to train the dataset.</p>

----

*   The linear regression model was able to predict the price of every diamond in the test set with an error of 869.38 of the real price.

*  The Decision Tree Regressor model was able to predict the price of every diamond in the test set with an error of 354 of the real price.

*  The Random Forest Regressor model was able to predict the price of every diamond in the test set with an error of 277

The best model was the Random Forest Regressor with accuracy score: 0.98
