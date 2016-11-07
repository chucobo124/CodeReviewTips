# When writing the Test case

* ### Don't duplicate the logic:

    It is really good to have a test case. But some of the test case is duplicate. It will be confuse when doing the code review and it will decrease the performance. So when every time we structure the test case. Please check it.

* ### The test case is obey to this web side in this moment: [better_rspec](https://www.google.com)

* ### Use Mock up than create a var

* ### Use one line testing code if you can:

   When you define a subject. This is very easy to write something like ```it{is_expected.to be true}``` this kind of test case line. It will be very clear to know what are we testing for.

* ### Merge the code as possible as you can:

   We need to merge some ```let(:something)``` or ```before``` as possible as you can. We are not prefer to add so many var or duplicate so many same action for it. Please make sure you code are clean. We also can merge when we create the ```factory girl```.
