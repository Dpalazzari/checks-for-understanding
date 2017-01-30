## Week One - Module 3 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. What is `json` and why is it important?
It is a form of javascript. It is important because it is easy for both humans and computers to read. JSON is useful for API's.

2. What's the difference between `joins` and `includes` in ActiveRecord?
joins connects one table to another. includes allows a detailed search of specified associations of a table that are loaded using the minimum possible number of queries.

3. What's an API?

Application Program Interface. This allows programs to consume other programs' data.

4. How do we test an internal API (in general)?

we visit the request, and test the JSON.parse value of the response.body.

5. What are two different ways to customize your `json`?

gem active_record_serializer and Jbuilder
