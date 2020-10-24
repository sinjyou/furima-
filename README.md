# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
## users テーブル

| Column             | Type   | Options  |
| ------------------ | ------ | -------- | 
| email              | string | NOT NULL |
| password           | string | NOT NULL |



## profile テーブル

| Column                | Type  |Options 
| ----------------------| ------| ------ 
| nickname              | string| NOT NULL| 
| email                 | string| NOT NULL|               
| password              | string| NOT NULL|         
| confirmation_password | string| NOT NULL|          
| family_name           | string| NOT NULL|           
| personal_name         | string| NOT NULL|  
| family_name_kana      | string| NOT NULL|  
| personal_name_kana    | string| NOT NULL|  
| Birth Year            | string| NOT NULL|  
| month of birth        | string| NOT NULL|  
| date of birth         | string| NOT NULL|  
## product テーブル

| Column           | Type   | Options |
| -----------------| -------|---------| 
| file selection   | string | NOT NULL|
| title            | string | NOT NULL|
| Description      | text   | NOT NULL|   
| Details_Category | string | NOT NULL| 
| Details_ Status  | string | NOT NULL|                      
| delivery_burden  | string | NOT NULL| 
| delivery_area    | string | NOT NULL| 
| delivery_Dsy     | date   | NOT NULL| 
| Selling price    | integer| NOT NULL| 

