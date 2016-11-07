# Code Review Tips

Overview: We do the code by testing during our code view. There is some tips need to be consider.

## When writing the code

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
    
## When writing the Test case

* ### Don't duplicate the logic:

    It is really good to have a test case. But some of the test case is duplicate. It will be confuse when doing the code review and it will decrease the performance. So when every time we structure the test case. Please check it.

* ### The test case is obey to this web side in this moment: [better_rspec](https://www.google.com)

* ### Use Mock up than create a var

* ### Use one line testing code if you can:

   When you define a subject. This is very easy to write something like ```it{is_expected.to be true}``` this kind of test case line. It will be very clear to know what are we testing for.

* ### Merge the code as possible as you can:

   We need to merge some ```let(:something)``` or ```before``` as possible as you can. We are not prefer to add so many var or duplicate so many same action for it. Please make sure you code are clean.
