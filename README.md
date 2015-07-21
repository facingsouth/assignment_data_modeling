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


Type of attributes


Relationships b/w entities


Convert into Tables

Normalize Data

























