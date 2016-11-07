# When writing the code

* ### Don’t make so many block in your code:

   There is some case like your ``` if ```  block and ```do while each ``` block. Please remember don't do so many this kind of block. It will decrease the performance.

* ### Find a method in the gem than create it:
   No matter this function is good or not. We prefer to use the origin method which the author created before. If you think that function is slow than what you should do is do a pull request to that author. And try your best to know all the structure of this gem.

* ### Make parameter when you define a function:
   This is an optional checking because when we add a parameter it is very easy to know what this function need for process. And sometimes it will protect the process if they do the wrong order to the code.

* ### Please check the code again after you done the structure:
   Sometimes we will write some code for structuring but some of them will be remove.Please check again to remove the one what is not using anymore.

* ### After Rubocop check the block:
   Rubocop will help you check the ```{}``` to ```do ... end``` but sometimes just a blank enter. Carefully check it to make it to be one line.

* ### mock up a request:
   When mock up a request. In the body params make it as {something}_response when you declare a var.

* ### Be careful your entire change:
   When we do the entire change sometime will change other bodies code. Please check it after you do it. You can do it in your github to check the diff.

* ### Define a function name should be a Verb and Really process that action:
   Define a function should be a verb that is really basic concept and also need to define it very clear, meaning we don't allow so a function but doing in different thing. etc: a function called ``` get_name ```.It should really <b>only</b> get the name not entire user profile.
