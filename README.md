<a id='intro'></a>
## Introduction

### Dataset Description 

I am investigating the data from the FBI's National Instant Criminal Background Check System. The NICS is used to determine whether a prospective buyer is eligible to buy firearms or explosives.The data has been supplemented with state level data from census.gov.

List of all column names in NICS table
1. month 2. state 3. permit 4. permit_recheck 5. handgun 6. long_gun 
7. other  8. multiple 9. admin 10. prepawn_handgun 11. prepawn_long_gun
12. prepawn_other 13. redemption_handgun 14. redemption_long_gun
15. redemption_other 16. returned_handgun 17. returned_long_gun
18. returned_other 19. rentals_handgun 20. rentals_long_gun
21. private_sale_handgun 22. private_sale_long_gun 23. private_sale_other
24. return_to_seller_handgun 25. return_to_seller_long_gun 26. return_to_seller_other 27. totals

List of all column names in census table

0   Fact          1   Fact Note      2   Alabama        3   Alaska         4   Arizona         
5   Arkansas      6   California     7   Colorado       8   Connecticut    9   Delaware      
10  Florida       11  Georgia        12  Hawaii         13  Idaho          14  Illinois        
15  Indiana       16  Iowa           17  Kansas         18  Kentucky       19  Louisiana       
20  Maine         21  Maryland       22  Massachusetts  23  Michigan       24  Minnesota       
25  Mississippi   26  Missouri       27  Montana        28  Nebraska       29  Nevada          
30  New Hampshire 31  New Jersey     32  New Mexico     33  New York       34  North Carolina  
35  North Dakota  36  Ohio           37  Oklahoma       38  Oregon         39  Pennsylvania    
40  Rhode Island  41  South Carolina 42  South Dakota   43  Tennessee      44  Texas           
45  Utah          46  Vermont        47  Virginia       48  Washington     49  West Virginia   
50  Wisconsin     51  Wyoming 

### Tables Discussion
1. Month column in NICS table runs from november 1998 to september 2017 but checking the fact row in census data, population estimates are only provided for 2010 and 2016. Therefore, there is a need to derive another table from NICS table that would contain 2010 and 2016 data which will be merged to census data.

2. Census data needs to ne transposed so that it can reflect the arrangement in the NCIS data.

3. Another observation is that in NCIS table, under state column, places like Virgina Island which are states in the US and they are not part of the states in the census table would be removed. 


4. Columns in both tables that are not relevant to the discussion will be removed.
 


### Question(s) for Analysis
###### 1. What is the gun per capita in all states in 2010 and 2016 respectively.
######  2. What is the trend in the types of gun purchased over time.

# [Google Collaboration Link] (https://colab.research.google.com/drive/1RfGmvkyx--XCBpo5iVzwRkUoafwH1q69?usp=sharing)