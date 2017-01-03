## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
Cookies are saved information that the website keeps in order to "remember" a User.
Google definition: "An HTTP cookie (also called web cookie, Internet cookie, browser cookie or simply cookie) is a small piece of data sent from a website and stored on the user's computer by the user's web browser while the user is browsing"

* What’s the difference between a session and a cookie?
A session is more of a timeframe of dialogue between two devices. 
Google Definition: "In computer science, in particular networking, a session is a semi-permanent interactive information interchange, also known as a dialogue, a conversation or a meeting, between two or more communicating devices, or between a computer and user (see Login session)."

* What’s a flash and when do you want to use flashes?
flash messages are displayed when a certain requirement is met. For instance, when a User successfully creates a comment, the flash[:success] message appears at the top of the screen. This tells the User that the action they just meant to complete, actually completed.

* Why do people say “HTTP is stateless”?
Every HTTP request is treated as a new request. The browser/server does not remember who you are when you come back for your second session.

* What’s authentication? Explain.
Authentication is basically checking to make sure the User is who they claim to be. If they know the email and password (which should be encrypted in the db) then they are authenticated as that user.

* What’s the difference between authentication and authorization?
Authorization is all about who can access what. If you have a website you don't want your Users to be able to access EVERYTHING, so you make it so only certain admin are AUTHORIZED to access certain information, html pages, etc

* What’s a before filter?
Before doing the thing, make sure this thing is true. essentially.

* How do we keep track of a user once they’ve logged in?
Once they log in, you start a session?

* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
You namespace a resource when you are authorizing, you nest a resource when the parent resource is REQUIRED to exist by the nested resource.

* At a high level, what tools can you use to implement authorization? How would you use them?
bcrypt gem and password_digest. Every User has a Password:password_digest and the gem one just needs to add to the Gemfile.

* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
From Ruby on Rails docs: "Declare an enum attribute where the values map to integers in the database, but can be queried by name"
So in the databse, the data is represented as a number (like 0 or 1). If the User has an enum number of zero then they would be considered a 'default' User, whereas a User with an enum number of 1 would be considered an 'admin'. This all depends on the fasct that the enum should be in the User model and look like this:
```
enum role: %w(default admin)
```
0 refers to index[0] of this array, and 1 represents index[1] of this array.

* What are some strategies you can use to keep your views DRY?
Helper methods(which are largely a mystery to me) and making sure you dont have too much logic in your views.

