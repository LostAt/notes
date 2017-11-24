# MySQL Date Stamps

```
2017-22-14 18:24:30
```

```
YYYY-MM-DD HH:MM:II
```
## Generate TimeStamp
```mysql
SELECT NOW();
```

# Example of UserRow being manipulated as an object

```php
$user = new User();
$user->email = 'test@test.com';
$user->save();
```

# Example Table Structure for Your Data

## user_table

id | email | contribution_id
--- | --- | ---
1 | adam@hotmail.com | 1
2 | wallace@hotmail.com | 2
3 | john.smith@gmail.co.uk | 5

## contribution_table

id | contribution | user_id | date_created
--- | --- | --- | ---
1 | 5.50 | 1 | 2017-11-24 08:00:00
2 | 7.33 | 1 | 2017-11-24 09:15:12
3 | 1.80 | 3 | 2017-11-24 09:16:55

## interest_rates
id | label | percent
--- | --- | ---
1 | Default | 1.5

## impact_constant
id | label | value
--- | --- | ----
1 | Default | 2.16

## revenue_amount_log
id | user_id | amount | date_created
--- | --- | --- | ---
1 | 1 | 12.83 | 2017-11-24 12:00:00

## total_revenue_amount_log
id | amount | date_created
--- | --- | ---
1 | 14.63 | 2017-11-24 12:00:00

# Example: Iterating through log entries

```php
foreach($log as $entry) {
    $results[] = $entry->amount * $impact_constant;
}
```

# Laravel (Start Here)

https://laravel.com/docs/5.5/installation#installation

# Coding Excersises

* TODO List App

```
todos = array();

while ($input !== "quit") {
   
   $input = getInput();
   
   if ($input == 'add') {
       addToTodoList();
   }
}
```
     
* Number Guessing Game
    
    * Generate a random number
    * wait for integer from user
    * tell if higher or lower than random no
    * if user guesses correct, end with WIN screen
    * if not, loop round

# PHP CLI (windows)

## 1. Set Local Path 

Seen as you have WAMP installed, there is nothing additional to install. However, setting an enviroment variable will make it easier for you. So you can type:

```
php myScript.php
```

Instead of

```
C:\Path\To\Php.exe myScript.php
```

See Top Answer here:
https://stackoverflow.com/questions/7361149/command-line-locally-using-wamp

## 2. Run a test script

Create this file somewhere:

test.php
```
<?php
    echo 'this is only a test!';
?>
```

run from same DIR
```
php test.php
```

You should see the messaged echoed into your CLI!
