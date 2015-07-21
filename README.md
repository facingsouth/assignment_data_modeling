# assignment_data_modeling
Mmmmm.... dataaaaa....

*Include your ERM modeling "pseudocode" in the space below*

Online Learning Platform

System Goals: Display Course listings, and lesson title and text

<!-- First EXERCISE -->

Entities (Models):
  Users, Courses, Lessons

Attributes
  Courses: id, title/name, description
  Lessons:  id title, text, course_id

Type of attributes
  id: integer
  title/name: VARCHAR(255)
  description: text
  text: text
  course_id: integer

Relationships b/w entities
  course has_many: lessons
  lesson belongs_to: course

Convert into Tables

Normalize Data

<!-- SECOND EXERCISE -->

Online Learning Platform

System Goals: Display Course listings, and lesson title and text

Entities (Models):
User, Profile


Attributes
  <!-- Users:   id, first name, last name, email, courses -->
User: id, username, email
Profile: id, city, state, country, age, gender, user_id

Type of attributes
id: integer
username: VARCHAR(255)
email: VARCHAR(255)
city: VARCHAR(20)
state: VARCHAR(20)
country: VARCHAR(20)
age: integer
gender: enum("Male", "Female", "Others")
user_id: integer


Relationships b/w entities
User has_one Profile
Profile has_one User

Convert into Tables

Normalize Data
Could put country, state, city in its own table.



<!-- THIRD EXERCISE -->

Message Board

System Goals: build a message board like Hacker News. Users can post links. Other users can comment on these submissions or comment on the comments.

Entities (Models):
User, Submission, Comment


Attributes
Users: user_id, username, email, crypted password
Submission: sub_id, user_id, link, title, post_time


Type of attributes


Relationships b/w entities


Convert into Tables

Normalize Data



<!-- Forth EXERCISE -->

E-commerce Site

System Goals: keep track of products, users, orders, shipments and all the bits and pieces necessary to glue them all together.

Entities (Models):
User, Product, Order, Shipment
user-address join table
product-order join table

Attributes
User: user_id, email, passwd
Address: address_id, street_number, street_name, city, state, country
Product: product_id, name, description, price
Order: order_id, user_id
Shipment: shipment_id, address_id(shipping address), order_id
user-address: user_id, address_id
product-order: product_id, order_id, quantity

Type of attributes
all_ids: int
User:
      email: varchar(20) 
      passwd: varchar(255)
Address:
      street_number: int 
      street_name:varchar(255) 
      city: varchar(20) 
      state: char(2) 
      country: varchar(20)
Product:
      name: varchar(20)
      description: text 
      price: decimal
Order: order_id, user_id
Shipment: shipment_id, address_id, order_id
user-address: user_id, address_id
product-order: product_id, order_id,
      quantity: int


Relationships b/w entities
User      has_many: Orders, Addresses

Address   has_many: Users, Shipments

Product   has_many: Orders

Order     has_many: Products, Shipments
          has_one:  Users

Shipment  has_one:  Addresses, Orders


Convert into Tables

Normalize Data





















