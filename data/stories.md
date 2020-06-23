## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Delhi"}
    - slot{"location": "Delhi"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"cuisine": "American"}  
    - slot{"price": "more than 700"}
    - slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}
    - utter_ask_sendmail
* affirm
    - utter_get_email
* email{"emailid": "bem.sama@gmail.com"}
    - slot{"emailid": "bem.sama@gmail.com"}
    - action_send_mail
    - utter_sent_email
* affirm
    - utter_goodbye
    - action_restart

## interactive_story_2
* greet
    - utter_greet
* restaurant_search{"location": "Delhi"}
    - slot{"location": "Delhi"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"cuisine": "American"}  
    - slot{"price": "more than 700"}
	- slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}
    - utter_ask_sendmail
* deny
    - utter_goodbye
    - action_restart
     
## interactive_story_3
* greet
    - utter_greet
* restaurant_search{"location": "Karaikudi"}
    - slot{"location": "Karaikudi"}
    - action_validate_location
    - slot{"loc_avl": "0"}
    - utter_ask_valid_location
* restaurant_search{"location": "Allahabad"}
    - slot{"location": "Allahabad"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"cuisine": "American"}  
    - slot{"price": "more than 700"}
	- slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}
    - utter_ask_sendmail
* affirm
    - utter_get_email
* email{"emailid": "bem.sama@gmail.com"}
    - slot{"emailid": "bem.sama@gmail.com"}
    - action_send_mail
    - utter_sent_email
* affirm
    - utter_goodbye
    - action_restart
   
## interactive_story_4
* greet
    - utter_greet
* restaurant_search{"location": "Karaikudi"}
    - slot{"location": "Karaikudi"}
    - action_validate_location
    - slot{"loc_avl": "0"}
    - utter_ask_valid_location
* restaurant_search{"location": "Allahabad"}
    - slot{"location": "Allahabad"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"cuisine": "American"}  
    - slot{"price": "more than 700"}
    - slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}	
    - utter_ask_sendmail
* affirm
    - utter_get_email
* deny
    - utter_goodbye
    - action_restart    

## interactive_story_5
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "mumzai"}
    - slot{"location": "mumzai"}
    - action_validate_location
    - slot{"loc_avl": "0"}
    - utter_ask_valid_location
* restaurant_search{"location": "Bangalore"}
    - slot{"location": "Bangalore"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}
    - slot{"location": "Bangalore"}
    - slot{"cuisine": "chinese"}
    - slot{"price": "more than 700"}
    - utter_ask_sendmail
    - utter_get_email
* email{"emailid": "bem.sama@gmail.com"}
    - slot{"emailid": "bem.sama@gmail.com"}
    - action_send_mail
    - utter_sent_email
* affirm
    - utter_goodbye
    - action_restart
	
## interactive_story_5
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "mumzai"}
    - slot{"location": "mumzai"}
    - action_validate_location
    - slot{"loc_avl": "0"}
    - utter_ask_valid_location
* restaurant_search{"location": "Bangalore"}
    - slot{"location": "Bangalore"}
    - action_validate_location
    - slot{"loc_avl": "1"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_validate_cuisine
    - slot{"csn_avl": "1"}
    - utter_ask_budget
* restaurant_search{"price": "more than 700"}
    - slot{"price": "more than 700"}
    - action_validate_price
    - slot{"prc_avl": "1"}
    - action_search_restaurants
    - slot{"emailbody": "Here are the top chinese restaurants in Bangalore for budget of more than 700"}
    - slot{"location": "Bangalore"}
    - slot{"cuisine": "chinese"}
    - slot{"price": "more than 700"}
    - utter_ask_sendmail
* deny
    - utter_goodbye
    - action_restart