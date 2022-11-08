# w3-database-project

## First Steps
### 1. Inspect the Data in each table, establish relationships between the tables.:
##### a) Table Film contains the columns : (film_id , title, description , release_year,  language_id  ,original_language_id , rental_duration ,rental_rate ,length  ,replacement_cost  ,rating ,special_feature , last_update) . It contains a column with only null values, being original_language_id
##### b) Table Actors contains the columns : (actor_id , first_name , last_name , last_update) It contains no null values
##### c) Table Category contains the columns : ( category_id, name, last_update) it contains no null values
##### d) Table Language contains the columns : (language_id , name, last_update) it contains no null values
##### e) Table Inventory contains the columns :(inventory_id, film_id , store_id , last_update)  it contains no null values
##### f)  Table Rental contains the columns : (rental_id , rental_date  , inventory_id  ,customer_id ,return_date  ,staff_id ,last_update)  it contains no null values
##### g) Table Old_HDD contains the columns : (first_name , last_name , title , release_year, category_id) it contains no null values
#### 2. establish relationships between the tables.
##### a) film_id is contained in the Table Film, Inventory . the relationship is one to many as each film_id can be contained many times in the table inventory
##### b) first_name last_name/ full_name is contained in the Table Actors and Old HDD, the relationship is one to many as each name is contained many times in the table Old HDD
##### c) category_id is contained in the Table Category, and Old_HDD  , the relationship is one to many as each category_id is contained many times in the table Old HDD
##### d) title is contained in the Table Film, Old_HDD, the relationship is one to many as each title is contained many times in the table Old HDD
##### e) language_id is contained in the Table Film, Language, the relationship is one to many as each language_id is contained many times in the table Film
##### f) inventory_id is contained in the Table Rental , Inventory the relationship is one to one 
### 2. Clean the data:
##### a) Table Film contains the columns original_language_id  that only has null values, we remove the column all together.
##### b) We remove all last_update columns in all dataframes
##### c) We change the data formats to date time where relevant
##### d) We downcast all tables if necessary
##### e) We concatenate the left name and right name and create a full name
##### f) create actors_id and film_id in old hhd with python




### 3a. Create database with create engine from jupyter notebook
### 3b. Create relationships between each dataframe(table) in SQL


![200187214-eb550106-8360-4746-9739-79d9131127ab](https://user-images.githubusercontent.com/114666478/200506149-b079e44c-bdbd-4f15-b204-a88820e2a6a6.png)




### 3c. From python export all dataframes with a connector to our sql database being careful of the order between the relationships


### 4. Create new database
### 5. Create queries






















