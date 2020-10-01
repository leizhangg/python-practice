
# Question
Your task is to write a simple program that would allow a user to compute the cost of a road trip with a car. User will enter the total distance to be traveled 
in miles along with the miles per gallon (MPG) information of the car he drives and the per gallon cost of gas. Using these 3 pieces of information you can 
compute the gas cost of the trip. User will also enter the number of days it will take to complete the trip. For each night (day-1 nights), user will need a hotel.
We will ask for the number of stars for the hotel the user wants to stay. 5 star hotel costs $250 per night. 4 star hotel costs $180 per night. 3 star hotel costs 
$120 per night, 2 star hotel costs $100 per night and finally 1 star hotel costs $50 per night. Using the hotel costs and the number of nights users will need to 
stay at a hotel, you can compute the hotel cost of the trip. Please note that 5 star and 4 star hotels give 10% discount if the user will be staying more than 2
nights -- (these are chain hotels, so even if you are staying at different locations discount apply). We should also account for the cost of meals. This depends 
on the type of hotel the user is staying. In general, we take 20% of hotel cost as the meal cost (after 10% hotel discount if applicable).

Example Run #1
Distance: 350
MPG : 15
Gas Price: 3.79
Days Traveling
Hotel Stars (1-5) : 3
Your total cost is $376.43333333333334

My solution;

!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Wed Sep 9 19:17:02 2020
@author: ZL
"""
distance = int(input())
mpg = int(input())
gas_price = float(input())
gas_cost = (distance/mpg)* gas_price
total_day = int (input())
total_night = total_day - 1
hotel_star = int(input())
hotel_cost = 0

if hotel_star == 5 and total_night > 2:
  hotel_cost = 250 - 0.9 * 250
elif hotel_star == 4 and total_night >2:
  hotel_cost = 180 - 0.9 * 180
elif hotel_star == 5:
  hotel_cost = 250
elif hotel_star == 4:
  hotel_cost = 180
elif hotel_star == 3:
  hotel_cost = 120
elif hotel_star == 2:
  hotel_cost = 100
else:
  hotel_cost = 50

meal_cost = 0.2 * hotel_cost
total_cost = gas_cost + (hotel_cost * total_night) + meal_cost * total_night

print ("Distance: ", distance,
"\nMPG: ", mpg,
"\nGas Price: ", gas_price,
"\nDays Traveling", total_day,
"\nHotel Stars(1-5)
: ", hotel_star,
"\nHotel Cost: ",hotel_cost,
"\nYour total cost is $",total_cost)
