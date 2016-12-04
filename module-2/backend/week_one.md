## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
GET: get to a webpage POST: add/interact to/with a webpage PUT: update a webpage's information DELETE: self explanatory

2. What is Sinatra?
Sinatra is the intermediary between the local machine and the web. It replicates a server?

4. What is MVC?
It is a way of building apps. A programmer should follow the Model View Controller convention.

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
There are a ton of files, and it makes it easier for people who haven't directly worked with the app to jump in and know 
what's going on.

6. What types of variables are accessible in our view templates without explicitly passing them?
Instance variables

7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
@count = params["count"] above the "erb :index" line
  
  ```ruby
  get '/horses' do
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
name = "Mr. Ed"
erb :index, :locals => {name: name}

9. What's the purpose of ERB?
To have your website displayed to a user in an easily readable and clear way using html and css (and js).

10. Why do I need a development AND test database?
Because when running your test suite you dont want it to take a million years to run everytime.

11. What's responsive design?


12. What is CRUD and why is it important?
C: create R: read U: update D: delete It basically covers all bases of functionality for a user when creating an app. 


13. What does HTTP stand for? 
Hyper Text Transfer Protocol

14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
<%= ruby code here %> and <% ruby code here %> I believe the interpolation with the = sign is used for interpolating ruby values that may have different values. They are not set.


15. What's an ORM?


16. What's the most commonly used ORM?
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
18. What's a migration? 
19. When you create a migration, does it automatically modify your database?
20. How does a model relate to a database?
21. What's the difference between agile workflow and waterfall method?
22. What is the difference between `#new` and `#create`?
