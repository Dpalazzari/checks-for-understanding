## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?

It is the inbetween for a database and a server. It is the ORM  that communicates/works with a SQL program. 

2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
They are Active record class methods. A car-dealership has_many cars. A Car belongs_to one car dealership.

3. What do they allow you to do?

They allow you to make relationships between databases.

4. What's the difference between agile workflow and waterfall method?

Agile workflow is all about building one full functionality at a time. All the way through, including the styling. Waterfall builds all aspects from the ground up at the same time.

5. What is the difference between `#new` and `#create`?

The new method needs to be saved. Create method does that automatically.

6. At a basic level, what does cURL allow you to do?

Had to look it up because I couldn't really remember. "cURL is a command line tool for getting or sending files using URL syntax"

7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.

They would probably have an intermediary table called 'students_teachers'. This table would have a student_id and a teacher_id because a teacher has_many students and a student has_many teachers.

8. Define foreign key, primary key, and schema.

The foreign key is the variable in a table that connects one table to another. For instance, In the car/dealership example from above the dealership_id in the car table is a foreign key whereas the car's id is considered a primary key. The schema is an rb file that shows the relationships between all tables. It also includes the name/type of every column in a table.

9. Describe the relationship between a foreign key on one table and a primary key on another table.
They are the same value, but there positions in the relationships are different.

10. What are the parts of an HTTP response?
VERB PATH PROTOCOL headers, body

11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
I'm not sure. It seems that when going through CRUD, it is very repetitive.


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
pluck is super useful. YOu can grab all the instances in a table with a specific column name. Ex: Student.all.pluck(:name)

2. Name your three favorite ActiveRecord rake tasks and describe what they do.
rake db:migrate - sets up your database
rake db:seed - parses real csv files into your dat tables...putting th emeat in the sandwhich.
rake db:test:prepare - because who DOESN'T like testing?

4. What can you expect from a group as you begin working together? As you continue working together?
There will be some differences in style and workflow. You will adjust to a group member's different work style as you become more experienced working with them. DTR is very important.

5. What two columns does `t.timestamps null: false` create in our database?
created_at and updated_at

8. What case does Ruby use for multi-word variables?
snake case!

9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
a teacher belongs_to a school, a school has_many teachers

10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
a teacher has a school_id(one to many)

