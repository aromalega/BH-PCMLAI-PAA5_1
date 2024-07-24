Problem Statement:
The goal is to Distinguish between customers who accepted a driving coupon versus those that did not.

Data:
This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, passenger, etc., and then asks people whether they will accept the coupon if they are the driver. Answers given that the users will drive there “right away” or “later before the coupon expires” are labeled as “Y = 1”, and answers “no, I do not want the coupon” are labeled as “Y = 0”. There are five different types of coupons—less expensive restaurants (under $20), coffee houses, carry out and take away, bars, and more expensive restaurants ($20–$50).

Deliverable:
Here's the link to my jupyter notebook
https://github.com/aromalega/BH-PCMLAI-PAA5_1/blob/3f7d8ce057f1a4a83b96484dbc71f693252f38fa/prompt.ipynb

Below are my findings
The percentage acceptance of coupons on entire data set is 56.8% with different coupons inorder from highest to lowest   
   - Coffee House, 
   - Restaurant(<20), 
   - Carry out & Take away, 
   - Bar, 
   - Restaurant(20-50)
     
![image](https://github.com/user-attachments/assets/e05d0a95-8f4a-45be-8b5b-509e1e8f2b0d)


I've analyzed the data further to see the various factors affecting the acceptance rate of these coupons

For Bar coupons,
The overall acceptance rate of bar coupons is 41%.
Among those, the acceptance rate is higher for frequent bar visitors and it remained almost within the same range with a slight decrease even when age above 25 and passanger(no kids) and occupations other than farming is considered. And slightly decreased for the drivers with low income (less than 50K) but is still higher than others.

For Coffee House coupons,
The percentage acceptance of coffee house coupons is about 50%. And it increases for the drivers
- Who go to coffee hose more often (more than 3 times a month)
- Age above 25
- Had an adult passanger
It doesn't look like weather had much affect on acceptance.
And the highest acceptance rate is at 10am.

![image](https://github.com/user-attachments/assets/b2ba998b-462e-4aeb-b652-02e1fc8054b4)


Since we've identified a few factors that affect the overall acceptance of coupons.
We can identify other factors that affect acceptance like 
- Different occupations
- Distance
- Education
- Number of children

We can further work on identifying the factors that affect the other coupons i.e.,
- Restaurant (<20)
- Restaurant (20-50)
- Carry Out & Take away
