# assignment_data_modeling
Mmmmm.... dataaaaa....

*Include your ERM modeling "pseudocode" in the space below*

Online Learning Platform

System Goals: Display Course listings, and lesson title and text

Entities (Models):
  Users, Courses, Lessons

Attributes
  <!-- Users:   id, first name, last name, email, courses -->
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



