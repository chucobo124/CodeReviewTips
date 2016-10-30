# Code Review Tips

Overview: We do the code by testing during our code view. There is some tips need to be consider.

## When writing the code

1. Don’t make so many block in your code:

     There is some case like your ``` if ```  block and ```do while each ``` block. Please remember don't do so many this kind of block. It will decrease the performance.

2. Find a method in the gem than create it:

    No matter this function is good or not. We prefer to use the origin method which the author created before. If you think that function is slow than what you should do is do a pull request to that author. And try your best to know all the structure of this gem.

3. Make parameter when you define a function:

   This is an optional checking because when we add a parameter it is very easy to know what this function need for process. And sometimes it will protect the process if they do the wrong order to the code.

## When writing the Test case

1. Don't duplicate the logic:

    It is really good to have a test case. But some of the test case is duplicate. It will be confuse when doing the code review and it will decrease the performance. So when every time we structure the test case. Please check it.

2. The test case is obey to this web side in this moment: [better_rspec](https://www.google.com)

3. Use Mock up than create a var

4. Use one line testing code if you can:

   When you define a subject. This is very easy to write something like ```it{is_expected.to be true}``` this kind of test case line. It will be very clear to know what are we testing for.
