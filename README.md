**********AWS Lex**********
Amazon Lex is a service for building conversational user interfaces (like chatbots) into everyday applications. In the past, developing tools like Lex have been incredibly complex, especially when one considers the power of Lex, allowing for the transcription, processing, and synthesis of text all via a few API calls. This project is a simple demo of Lex chatbot and how it can be used to process voice input and act on a users input (refereed to as utterances).


**********Setup**********
In order to use Amazon Lex, you must have an active AWS account (with billing information entered). You will need to create an IAM user with programmatic access, and access to both Lex  and AmazonLexFullAccess.


**********Core Concepts and Terminologies**********

1) Intent – An intent represents an action that the user wants to perform. You create a bot to support one or more related intents. For example, you might create a bot that orders burgers and drinks. For each intent, you provide the following required information:

   Intent name– A descriptive name for the intent. For example, OrderFoodIntent. Intent names must be unique within your account.

2) Sample utterances – How a user might convey the intent. For example, a user might say "Can I order a Burger please" or "I want to order a Burger".

3) Slot – An intent can require zero or more slots or parameters. You add slots as part of the intent configuration. At runtime, Amazon Lex prompts the user for specific slot values. The user must provide values for all required slots before Amazon Lex can fulfill the intent.

4) Slot type – Each slot has a type. You can create your custom slot types or use built-in slot types. Each slot type must have a unique name within your account. For example, you might create and use the following slot types for the OrderFoodIntent intent:
 
    FoodType – With enumeration values : Veg Burger , Devil Veg Burger , Royal Veg Burger.
    Sides – With enumeration values : French Fries , Cold drink .


**********Project Working**********
  
-->  So , First of all we invoke the bot  by sending a message as "hi" , "hello" , "hey" etc. 
-->  Bot will reply back with a message "What type of food you want to order? " You will get 3 options i.e "Veg Burger , Devil Veg Burger and Royal Veg Burger". You choose any one option and either type the same or just click that button.
-->  Then it will ask for "What type of Patty do you want to have? " . You will get  2 options i.e  "Single Patty or Double Patty". You choose any one.
-->  Further it will ask for "Would you like to have extras? " . You will get 3 options i.e "Extra Cheese , Extra Mayonnaise or No extras". You choose any one.
-->  Then it will ask for "Would you like to have add on Sides? " which includes 3 options i.e "French Fries, Cold Drink , No sides" . You choose any one.
-->  Then the bot will ask your personal details which includes "First Name" ,  "Contact Number" .
-->  After that it will ask your preffered delivery time for your order .
-->  Bot will ask for confirmation of your order with your order details . If its okay then type "Yes" for confirming your order and if its not okay then type "No" and your order will be cancelled.
-->  If the order details are okay then it will give a confirmation message that "Your order was confirmed and will be delivered to you on time".



*************************************************************************Thank You**************************************************************************



 
