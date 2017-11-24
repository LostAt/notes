user table
----------
id
email
contribution_id

contribution_table
------------------
id
contribution (gbp)
user_id
date_created
date_updated


interest_rates
--------------
id
label
percent

impact_constant
---------------
id
label
value

revenue_amount_log (cron job 1day)
----------------
id
user_id
amount        - 466
date_created


foreach($log as $entry) {
    $results[] = $entry->amount * $impact_constant;
}

total_revenue_amount_log
------------------------
id
amount
date_created



https://laravel.com/docs/5.5/installation#installation



User Interface

--> request 

Application

/graph

  getGraph()

   $user->getRevenueLog()
   
   $i = $this->getImpactConstant()

Database


********

TODO List App
-------------

TODO ARRAY

WHILE LOOP() 
    WAIT FOR INPUT
    
    if (input == add)
    
    
    
Number Guessing Game
--------------------




PHP CLI (windows)






2017-22-14 18:24:30
YYYY-MM-DD HH:MM:II




$user = new User();
$user->email = 'test@test.com';
$user->save();


NOW()




user->contribution
