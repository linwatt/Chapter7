It’s not enough to simply have different layouts for different devices. You also need **different Java code** to run alongside the layouts so that the app can behave differently depending on the device. In our Workout app, for instance, we need to provide **one activity for tablets, and two activities for phones**.

TO AVOID DUPLICATE CODE
The second activity that runs only on phones will need to insert the details of a workout into the layout. But that code will also need to be available in the main activity for when the app is running on a tablet. The same code needs to be run by multiple activities. Rather than duplicate the code in the two activities, we can use fragments. So what’s a fragment?
