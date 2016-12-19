# Active View
  * ### The Form Builder
    The <b>FormBuilder</b> can give you some method to create the view.

    This is the basic example of [FormBuilder](http://api.rubyonrails.org/classes/ActionView/Helpers/FormBuilder.html)

    There are some step to build your view.

    1. Create your ```from_for``` block
    2. Create your ```CustomizeBuilder```class and inherit ```ActionView::Helpers::FormBuilder```
    3. Add the ```CustomizeBuilder``` in builder condition.

  * ### How to use Ajax to control a partial view
    There is the explain in [Rails Doc](http://guides.rubyonrails.org/working_with_javascript_in_rails.html) .

    The Basic logic is in the javascript which is gonna use it's features to make a partial render without reload page.

  * ### How to break line in haml
    There is the example of [Haml break line](http://haml.info/docs/yardoc/file.FAQ.html#q-multiline)
    The Haml Syntax force you have the formate with Haml role. Like space and blank or the style of code. Then I got the problem is I need to break line when I have long Ruby code. The basic break line syntax is ```|``` symbol here is the example.
    ```Ruby
    = select_tag "parent_taxon",options_run from_collection_for_select(Taxon.where.not(parent_id: nil).order('name ASC'), "id", "name")
    ```
    OK , we can get the result when we need all parent taxon but there is one thing is wrong is this line is corse the screen line which is no good. The way add break line to haml is like this.
    ```Ruby
    = select_tag "parent_taxon",                       |
                   options_from_collection_for_select( |
                   Taxon.where.not(parent_id: nil)     |
                   .order('name ASC'), "id", "name")   |
    ```
    Make sure ```|``` should be align or we will got error.
