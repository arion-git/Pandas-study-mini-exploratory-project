# Pandas study mini exploratory project

# Tasks

1. Import the `pandas` library as `pd`. Upload `bookings.csv` dataset 
        with separator - `;` .
        Check the table size, variable types, and then print the first 7 lines 
        to look at the data.
2. Change the column names to lowercase and replace spaces with underscores. 
3. Users from which countries have made the most successful bookings? 
        Specify the top 5.
4. How many nights on average are booked in different types of hotels
5. Sometimes the type of room received by the client ( `assigned_room_type` ) 
        differs from the one originally booked ( `reserved_room_type` ). 
        This can happen, for example, due to overbooking. 
        How many such observations were found in the dataset?
6. Review your planned arrival dates.
        - What month was the most successful booking in 2016? 
            Has the most popular month changed in 2017?
        - Group the data by years and check which month City Hotel bookings 
            were canceled the most in each period.
7. Look at the numerical characteristics of the three variables: 
        `adults`, `children` and `babies`. Which one has the largest average value?
8. Create a `total_kids` column by concatenating `children` and `babies`. 
        What types of hotels, on average, are more popular with clients with children?
9. Create a `has_kids` variable that takes the value `True` if the client specified 
        at least one child during the booking ( `total_kids`), and `False` otherwise. 
        Calculate the ratio of the number of users who left to 
        the total number of customers, expressed as a percentage (`churn rate`). 
        Indicate which group has the highest rate.

# Data Description

**There are the following variables:**

* Hotel - hotel type (City Hotel or Resort Hotel)
* Is canceled - the booking was canceled (1) or not (0); 
        what is not canceled is considered successful
* Lead time - the number of days elapsed between the date of booking 
        and the date of arrival 
* Arrival full date
* Arrival date year - year of arrival
* Arrival date month - month of arrival
* Arrival date week number - arrival week number
* Arrival date day of month - day of arrival
* Stays in weekend nights - the number of days off (Saturday or Sunday) 
        that the guest has booked to stay at the hotel
* Stays in week nights - the number of days (from Monday to Friday) 
        that the guest has booked to stay at the hotel
* Stays total nights - total number of nights booked 
        (sum of the two previous columns)
* Adults - number of adults
* Children - number of children
* Babies - number of babies
* Meal - selected type of food
* Country - client's country of origin
* Reserved room type - reserved room type
* Assigned room type - type of room received (may differ from booked)
* Customer type - booking type
* Reservation status - value of the last reservation status: 
        Canceled - was canceled by the client; 
        Check-Out - the client has checked in, but has already left the hotel; 
        No-Show - the client did not register and informed 
        the hotel administration the reason
* Reservation status date - Status update date