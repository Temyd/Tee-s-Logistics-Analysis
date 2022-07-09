# Tee's-Logistics-Analysis
<img width="548" alt="intro car" src="https://user-images.githubusercontent.com/105246702/178114119-a45b1f96-d1ce-46fd-ba43-3972a8060fd3.png">


# Introduction
A project to showcase what I learnt Day 17 of #NG30daysoflearning. 'Creating a Dashboard and publishing to PowerBi Service by [Theoyinbooke](https://twitter.com/TheOyinbooke?s=20&t=lOOFsBn0xfKw8ud_FJf2Jg)

# Introduction
Pelumi a fresh graduate from the University is interested in getting a car, she is torn between getting the car this month or getting it later next year.
She started researching what will be the best option for her. 
She then remembered me, her best friend who is currently undergoing the Data Analytics track training for the #NG30daysoflearning. She sent a dataset to me, and told me to derive meaningful insights that will help her make a decision in getting a car. 

I went through the dataset. Thus the big question that need answer to is **"Can we Predict the Price of the Car She wants to buy?"** Bearing in mind that due to the high cost of new cars, most people tend to be able to afford Used Cars. Thus there is a need to be able to predict the selling price of the used cars

# Data Sourcing
Data was provided in the raw form and can be gotten [here](https://raw.githubusercontent.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/main/KaggleCarData.csv)

# Data Transfprmation
- Data was gotten from the web and exported into Excel
- In Excel, I created a new column showing the cars age (Current year'2022' - Car's year'Year of the car when it was bought'
- I then loaded into PowerBi from Excel, Where i did futher transformations in Power Qwery
- In Power Qwery, I made sure my data types were correct and every other parameters was appropriate
- After which it was loaded into PowerBi 
- In PowerBi I created a DAX measure to show the Average Cost saved (Average Present price - Average Selling price)
- It was then ready for Analysis and Visualisation

### Before moving on, there is a need to understand the Column names which will make understanding the analysis easier

- Car_Name: Name of the cars.

- Year: Year of the car when it was bought.

- Selling_Price: Price at which the car is being sold.

- Present_Price: Current showroom price of the car.

- Kms_Driven: Distance completed by the car in km.

- Fuel_Type: Fuel type of the car i.e Diesel,Petrol,CNG

- Seller_Type: Tells if a seller is a dealer or an individual.

- Transmission: If the car is manual or automatic.

- Owner: Number of owners the car has previously had

     0 'No previous owners'
    
     1 '1 previous owner'
    
     2 '2 previous owners'
    
     3 '3 previous owners'
     

# Data Visualisation
[Interact with dashboard here]()

# Findings
### Dealers offer a higher selling price
We have two seller types "Individual and Dealers". Selling price of car is higher when sold by Dealers compared to buying from an Individual.
Futher research shows The reason is simple: While a dealer needs to make a profit on each vehicle, a private seller doesn't have the same concern. Instead, private sellers are usually trying to sell an old vehicle so they can buy a new one, and that means they're often more willing to negotiate just to ensure that the car is sold quickly. 
<img width="322" alt="selle type" src="https://user-images.githubusercontent.com/105246702/178114298-a29c6571-23b6-47a1-b0bf-c113cc0c4914.png">


### A car with no previous owners or 3 which is more expensive?
A car with no previous owner or maybe 1 is definitely more expensive than a car with 3 previous owners. Which brings us to a conclusion that "The lesser the previous owners, the higher the selling price"

_The dataset had missing values for 2 owners_
<img width="366" alt="owners" src="https://user-images.githubusercontent.com/105246702/178114317-18334817-ce50-4781-bba9-9ccc4770ddfa.png">


### Mannual Cars are cheaper
The insight gotten from the selling price of both mannual and automatic cars, showed that the company sold more mannual cars, which is an indication that it is cheaper compared to automatic cars
<img width="364" alt="mode of trans" src="https://user-images.githubusercontent.com/105246702/178114360-1ed7810a-e211-467f-8388-490cf853bec7.png">


### A car that uses Petrol is more affordable
We have 3 major souce of fuel type in our dataset; Petrol, Diesel and CNG "Compressed Natural Gas". Our Analysis showed the company sold more Petrol fuel type cars, which is an indication it has lesser selling price compared to the others.

Petrol Cars are the most affordable amongst the 3, Why is this so?
- Fuel Cost: The Petrol fuel costs a less cpmpared to diesel and CNG more.
- Driving Experience: Diesel engines are mighty. These offer higher torque, ensuring a smooth driving experience for the car owner. This makes diesel cars more expensive
- Servicing Costs: Servicing a Petrol car is less expensive than Diesel cars and CNG.
- Insurance Cost: Car experts know that diesel cars cost around 10 to 15% more than petrol cars.
Futher research shows that Currently, in Nigeria, we have less than five CNG plants available for refilling purposes. And a reaserach from 2015 states that there are about 5,000 CNG cars in Nigeria. This means its not readily available thus putting it on the high side compared to Petrol cars.

<img width="322" alt="fuel type" src="https://user-images.githubusercontent.com/105246702/178114463-48c0a377-4111-4abe-b571-f65a65e0411b.png">


### Selling Price and Current Price have a positive relationship
As the Present price of a car increases the selling price also tends to increase which shows a  Positive linear correlation.
<img width="347" alt="sp vs pp" src="https://user-images.githubusercontent.com/105246702/178114482-43b376bc-e7f4-4e82-b26a-d09c0aa05c2f.png">


### The Lesser the kilometers(Km) driven the more expensive the car is
The lesser a car has been driven the more expensive it is. 
<img width="340" alt="km drive" src="https://user-images.githubusercontent.com/105246702/178114511-ff2bd32e-f812-4d86-9bc1-87277d3c0847.png">


### The Car's Age has something to say about the selling price,
Our analysis showed that the younger the car, the higher the selling price
<img width="349" alt="car age" src="https://user-images.githubusercontent.com/105246702/178114519-1b62afb2-86e5-45c3-9818-f6d819ae4103.png">


### Cost Saved
When thinking of buying a car, one might be caught between buying a new or used car based on available funds. Analysis shows that on average about 707.73 dollars is saved when one goes for a used car.
<img width="544" alt="cost saved" src="https://user-images.githubusercontent.com/105246702/178114527-910b0552-dda1-4c05-87c1-834bbf9098f6.png">


    
