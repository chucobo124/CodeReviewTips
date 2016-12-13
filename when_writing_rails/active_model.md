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

* ### Has one method in Model
    When we add the method ```has_one```. This will going to make many to one or one to one relation and there is another usage. Let's take this situation. We already have many product were using one to many relation to picture. Then there is a product call SpeciaProduct are only have one to one relation to picture. In this case we create a type to separate Product and SpecialProduct. So what about the picture which are already use the one to many relation ?

    The has_one function will only take the last one which is the newest picture. So when I call ```Product.picture```. It will become the latest picture when I call it.
