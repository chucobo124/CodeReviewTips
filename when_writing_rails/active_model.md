# Active Model

* ### [The different between include and join.](http://tomdallimore.com/blog/includes-vs-joins-in-rails-when-and-where/)

* ### Database Control
  When doing the database control. there are some tips I will forgot is the multiple search and multiple insert.
  #### - Multiple Search
    The multiple search we can use array in the where function
    ``` Ruby
    FieldAction.where(affiliate_id: affiliate_id,
                     field: %w(image_url_2
                               image_url_3
                               image_url_4
                               image_url_5)).destroy_all
    # This will output an array so we can also doing destroy_all method
    ```
  #### - Multiple Insert
    This one is using for a big number of information, such like a big number of profile.
    ``` Ruby
    User.create([{username: 'Lucas', age: 10},
                 {username: 'Nancy', age: 11},
                 {username: 'Elan', age: 12}])
    # Make your multiple array with correct 
  ```
