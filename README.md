# Analysis-of-online-food-delivery-Rating

We analysed the dataset comprised of various features like deliveryTime, orderTime, TIP, ST etc. <br >
Our analysis consist verious steps:<br >
 > 1. Data loading<br >
 > 2. Data Handling & Missing value replace<br >
 > 3. EDA analysis : Univariate & Multivariate analysis<br >
 > 4. Feature Selection with Backward Feature selecion method<br >
 > 5. Linear regression model using scikit learn library<br ><br ><br >
  
**Detailed Explaination**:<br >

Data Quality   - <br ><br >
========================<br >
>duplicate  records <br >
>target label missing <br >
>data integrity  <br >
>>	order time and delivery time check <br >
>>	negative distance <br >
>>	rating check - zero value acceptable  <br ><br >
	     
>missing values 
>>	discount  - replace with zero  <br >
>>	delivery charges - replace with zero  <br >
>>	surge charges - replace with zero <br >
>>	packagind charges - replace with zero <br >
>>	tip - replace with zero <br >
>>	order id - replace with some unique value or drop it <br >
>>	promo code - - replace with new category <br >

Data Transformation<br >
========================<br >
>To be computed <br >
>>	Delivery time requird for actual delivery in minutes   - from DateTime and Delivery Time <br >
>>	Bill amount from Cost - Discount + Delivery charges + Surge charges + Packaging charges	+ ST + Tip    <br > 
>>	Order type - veg / nonveg / mix from Items    <br ><br >

>To be converted  <br >
>>	Status to binary 0 /1 <br >

>Dummy variables<br > 
>>	PromoCode<br >
>>	Payment mode<br ><br ><br >
>>	Membership<br ><br >

>>Normalization of numeric columns <br ><br >

>Data Reduction <br >
>>To be dropped <br >      
	ID<br >
	Provider<br >
	DateTime<br >
	Delivery Time<br >
	PromoCode<br >
	Payment mode<br >
	Items<br >
	Membership<br >

EDA <br >
========================<br >
Univariate analysis  of each attribute<br >
	Packaging charges - same values - can be dropped<br >
	ST - same values - can be dropped<br ><br >

Coorelation between predictors <br >
>>find and drop highly correlated attribtues<br >
>>	Distance and delivery charges<br >
>>	 Bill amount and cost<br ><br >

		
Feature selection and Modeling  <br >
==================================<br >
Backward stepwise feature elimination<br ><br >
		
Model explanation <br >
=====================<br >
Generalized model obtained with good accuracy <br >
Comparison of model parameters done with observations from EDA<br >


  
