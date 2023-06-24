# Orbital-2023
Bot Description: 
Brief overview
GrabShare Bot helps users look for other users to split cost on their Grab food orders and transport trips. Users can choose to start/join Grab group orders/transport trips to order or travel with others to save money on delivery and petrol.


Bot Setup: 
How to set up and configure the Telegram bot. 
Start a chat with BotFather on Telegram.
Use command /newbot and follow the instructions given by BotFather to get the bot token for the new bot.
Change the value of BOT_TOKEN (line 34) to the bot token obtained.
Run "python <location>\\<location>\\...\\grabshare_bot\\grabshare_bot.py" in Terminal.


Usage: 
/start: Begin your search for similar food orders or transport trips
User is prompted with "Food" or "Transport" keyboard buttons to choose if they want to order food or travel.

If user chooses "Food",
user is prompted with "Start an order" or "Join an order" keyboard buttons.
If user chooses to "Start an order",
user is asked to input the following details of their food order.
a) postal code of the delivery location
b) restaurant name
c) Grab group order link
d) order send-off time, where user is prompted with 4 keyboard buttons in 15 minute intervals from their time of order creation
Note: users are only allowed to start food orders that will be sent off by 2359 on the day of creation.
If user chooses to "Join an order",
user is asked to input their delivery location. The bot will then show the user orders with delivery locations within 1 km of the user within the same day in the following format:
Location: <postal code>
Order started by: @<username of order-starting user>
Restaurant name:
Link:
Order closes at:
User can then make their decision and join the order using the Grab group order link or contact the order-starting user for further details.

If user chooses "Transport",
user is prompted with "Start a trip" or "Join a trip" keyboard buttons.
If user chooses to "Start a trip",
user is asked to input the following details of their transport trip.
a) pick up postal code
b) drop off postal code
c) departure time
Note: users are only allowed to start transport trips that will depart by 2359 on the day of creation.
If user chooses to "Join a trip",
user is asked to input their pick up and drop off postal codes. The bot will then show the user orders with pick up and drop off postal codes within 1 km of the user's within the same day in the following format:
Pick-up: <Pick-up postal code>
Drop-off: <Drop-off postal code>
Departs at:

Users are only allowed to have a maximum of 1 food order and 1 transport order going on at the same time.


Common issues:
When keying information, any mistakes cannot be corrected immediately. Users can use /start and key in the all information again. It is a little troublesome, but it won't take long.
