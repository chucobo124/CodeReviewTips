# Active Admin
  * ### How to Customize your Filter Side Bar
     #### - Build your own Side Bar
     ```Ruby
      config.clear_sidebar_sections!
      sidebar :filters do
        render partial: 'search'
      end
     ```
     The first line ```config.clear_sidebar_sections!``` is going to remove the filter which generate in default. The sidebar function can help you render the partial page. The partial structure is the same as rails.

     - The example is refer to github [repo](https://gist.github.com/dmitry/4240801)

     - The explain of [<b>ActiveAdmin</b>](http://activeadmin.info/docs/6-show-pages.html)

    #### - About the Forms
    The ActiveAdmin can use [Formtastic](https://github.com/justinfrench/formtastic) gem.
