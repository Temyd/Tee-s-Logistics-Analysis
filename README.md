# Tee's-Logistics-Analysis
<img width="548" alt="intro car" src="https://user-images.githubusercontent.com/105246702/178114119-a45b1f96-d1ce-46fd-ba43-3972a8060fd3.png">


# Introduction
A project to showcase what I learnt Day 17 of #NG30daysoflearning. 'Creating a Dashboard and publishing to PowerBi Service by [Theoyinbooke](https://twitter.com/TheOyinbooke?s=20&t=lOOFsBn0xfKw8ud_FJf2Jg).
The major goal was to Publish on the PowerBi service and also create a dashboard the stakeholders would be interested in seeing. One thing I was also able to learn along the way is the use of PowerBi to make predictions.

# Problem Statement
Pelu a working class woman, decided one of her new year resolutions is to get herself a car. However research tells us that due to the High price of new cars and lack of funds by customers, the sales of used cars is on the increase. Having known this as a Data Analyst, I want to help Pelu predict the prices of cars in the coming months or years so she will know how to plan her budget.

# Data Sourcing
Data was provided in the raw form and can be gotten [here](https://raw.githubusercontent.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/main/KaggleCarData.csv)

# Data Transformation
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
I published my report to PowerBi Service and also created a dashboard to show specific visuals I want the stakeholders to see.
<img width="638" alt="car analysis" src="https://user-images.githubusercontent.com/105246702/178162633-ab1de210-6c30-4cb3-83c2-6ac8c0d8209d.png">

[Interact with dashboard here](https://app.powerbi.com/view?r=eyJrIjoiYTI5ZTU2OTctNWI5Yi00Y2M0LTk2NmQtMzRjNDM5Zjc3MjNkIiwidCI6IjBjZmU3YmI2LTZhMzUtNDM4OS1hODQ4LTU1ZTdjZjZlN2NmMSJ9&pageName=ReportSectionc2281e68380e7003ca98)

# Findings
### Dealers offer a higher selling price
We have two seller types "Individual and Dealers". Selling price of car is higher when sold by Dealers compared to buying from an Individual.
Futher research shows The reason is simple: While a dealer needs to make a profit on each vehicle, a private seller doesn't have the same concern. Instead, private sellers are usually trying to sell an old vehicle so they can buy a new one, and that means they're often more willing to negotiate just to ensure that the car is sold quickly. 

<img width="322" alt="selle type" src="https://user-images.githubusercontent.com/105246702/178114298-a29c6571-23b6-47a1-b0bf-c113cc0c4914.png">


### Depreciation in value affects selling price
A car with no previous owner or maybe 1 is definitely more expensive than a car with 3 previous owners. Which brings us to a conclusion that "The lesser the previous owners, the higher the selling price". This can also be linked to depreciation in value of used cars. The more the previous owners, the higher the depreciation value.

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
As the Present price of a car increases the selling price also tends to increase which shows a  Positive linear correlation. It should be noted that due to the present economic situation globally, there is a possibility present prices of cars will keep increasing which means the selling price also increases.

<img width="344" alt="km drive" src="https://user-images.githubusercontent.com/105246702/178146933-324a632b-22d3-4d9a-b128-94b49e7f6292.png">


### The Lesser the kilometers(Km) driven the more expensive the car is
The lesser a car has been driven the more expensive it is. 

<img width="346" alt="sp vs pp" src="https://user-images.githubusercontent.com/105246702/178146940-882bcf0e-c988-4e96-ab1e-af84972f12f6.png">


### The Car's Age has something to say about the selling price,
Our analysis showed that the younger the car, the higher the selling price

<img width="349" alt="car age" src="https://user-images.githubusercontent.com/105246702/178114519-1b62afb2-86e5-45c3-9818-f6d819ae4103.png">


### Cost Saved
When thinking of buying a car, one might be caught between buying a new or used car based on available funds. Analysis shows that on average about 707.73 dollars is saved when one goes for a used car.

<img width="544" alt="cost saved" src="https://user-images.githubusercontent.com/105246702/178114527-910b0552-dda1-4c05-87c1-834bbf9098f6.png">

# Conclusion
- Present Price of a car plays an important role in predicting the Selling price, as one increases the other increases as well
- Car age affects the selling price negatively, as the car ages the selling price reduces
- Car with Petrol fuel type is more affordable
- Car of Mannual type is less expensive compared to Automatic
- Buying a car from an Individual is more Affordable than buying from a Dealer.
- Car with lesser previous owners are more expensive

# What should be done
- Anyone interested in getting a car, should get it as soon as possible, because of the unstable economy there is a possibility the present price will increase thus an increase in selling price.
- In as much that it is cheaper getting from an individual, it is not adviseable, a dealer will be better cos they have a reputation to protect.
- The more the previous owners, the more depreciated in value the car is, its adviceable to go for a car with no or just 1 previous owner, though the cost might be high.
