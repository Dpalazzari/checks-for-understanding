## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
rails new project_name_here"

2. What do Models generally inherit from in rails?
active record

3. What do Controllers generally inherit from in a rails project?
application controller

4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
get 'horses' => 'horse#show' OR resources :horses, only: [:show]

5. What rake task is useful when looking at routes, and what information does it give you?
rake routes tells you all the wonderful routes you have available to you

6. What is an example of a route helper? When would you use them?
nested routes. When things can't exist without other things it would be useful to have nested routes

7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
I always know when I see the error, but after Job Tracker all weekend I can't for the life of me think of why

8. What are strong params and why are the necessary?
it is a private method in your controller that makes it so people can't alter the html and params when forms are submitted.

9. What role does `form_for` play in helping us create our forms?
it creates a form for a specific object i.e. @comments, @contacts, @jobs, etc

10. How does `form_for` know where to submit the user's input?
In the controller

11. Create a form using a `form_for` helper to create a new `Horse`. 
<%= form_for @horses do |f| %>

<%= f.label :name %>
<%= f.text_field :name %>

<%= f.label :age %>
<%= f.number_field :age%>

<%= f.submit %>

12. Why do we want to validate our models?
Makes sure all relationships are working and we can't create an object without the required attributes/columns(in the database)
