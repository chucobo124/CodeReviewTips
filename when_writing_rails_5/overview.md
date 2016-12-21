# About Rails 5

There is one thin I really interesting which is API mode of rails 5. In the pass. When we wanna create an API server in Rails we need to install grape. This time rails 5 release API server to independent the rails server. Really interesting. And [Rails documentation](http://edgeguides.rubyonrails.org/api_app.html) already wrote the article to explain how api server works.

# What's new stuff

* ### ApplicationCable

  Create a real time action in your application.

  [Link to documentation](http://edgeguides.rubyonrails.org/action_cable_overview.html)

* ### ApplicationJob

* ### ApplicationMailer

* ### ApplicationRecord
  #### - The abstract in model
  Interesting. There is a abstract type in Model. Will it be the same like how we implement in Java ? But the answer is <b>No</b>. So what is this doing in model. There is a new line when we create a application.

  ```ruby
  class ApplicationRecord < ActiveRecord::Base
    self.abstract_class = true
  end
  ```
  This line is helping to inherit to the ActiveRecord when you wanna have a function in the ```ActiveRecord```.

  [Link to documentation](http://blog.bigbinary.com/2015/12/28/application-record-in-rails-5.html)

* ### Api Mode
```shell
rails new my_api --api
```
According the command line. Our application will become API mode. There are some thing different than origin rails app.

 <b>1. Controller</b>

    Beforehand. The Controller will going to inherit. ```ActionController::API``` than ```ApplicationController```

 <b>2. application.rb </b>
   ```ruby
   config.api_only = true
   ```
   This line will add it to define this app as API mode.

  [Link to documentation](http://edgeguides.rubyonrails.org/api_app.html)
