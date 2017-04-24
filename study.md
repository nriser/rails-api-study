# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsibilities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model layer consists of ruby classes provided by Rails. It is responsible
for finding, creating, and saving data in a database, so that developers do not
have to communicate with the database directly using SQL. Models are ruby
classes.
```

## Define Controller Responsibilities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer is responsible for taking user input, calling the
appropriate models, and then passing output to the view.
```

## Define Router Responsibilities

In your own words, define what the router does in Rails.

```md
The router tells the server which controller to activate.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
1. Browser makes a GET request to a particular URL
2. Web server receives the request and activates the router, which then tells
the server which controller to activate.
3. Controller parses the user requests, calls the appropriate model
4. Model communicates with the database to perform the user request and returns
back the output to the controller.
5. Controller passes the output onto the View so that the user can see
the result in the browser
```
