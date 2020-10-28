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

* Deployment instructions4

* ...
## users テーブル


NOT NUL
| Column                | Type  |Options 
| ----------------------| ------| ------ 
| nickname              | string| nul:false | 
| email                 | string| nul:false,unique:true|           
| password              | string| nul:false|         
| confirmation_password | string| nul:false|          
| family_name           | string| nul:false|           
| personal_name         | string| nul:false|  
| family_name_kana      | string| nul:false|  
| personal_name_kana    | string| nul:false|  
| Birthday              | date| NOT NULL|  

Association
・belongs＿to_hash :Birthday
・belongs＿to_hash :prefecture
・has_many :products
・has_many :Purchase

## product テーブル

| Column           | Type   | Options |
| -----------------| -------|---------| 
| file selection   | string | nul:false|
| title            | string | nul:false|
| explain          | text   | nul:false|   
| Category         | string | nul:false| 
| Status           | string | nul:false|                      
| postage          | string | nul:false| 
| prefecture       | string | nul:false| 
| delivery_Dsy     | date   | nul:false| 
| Selling price    | integer| nul:false| 

Association

・belongs_to_active_hash :category
・belongs_to_active_hash :status
・belongs_to_active_hash :delivery_days
・belongs_to :user
・add＿index products,:name
## Purchase テーブル

| Column           | Type   | Options |
| -----------------| -------|---------| 
| zop_code1   　　　| string | nul:false|
| prefecture_id    | string | nul:false|
| city          　　| text   | nul:false|   
| address1         | string | nul:false| 
| address2         | string | nul:false|                      
| postage          | string | nul:false| 
| prefecture       | string | nul:false| 
| delivery_Dsy     | date   | nul:false| 
| Selling price    | integer| nul:false| 
| phone            | integer| nil:false|

Association
・belongs to:user

