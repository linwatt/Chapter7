Before an activity can talk to its fragment, the activity first needs to get a reference to it. To get a reference to the fragment, you first get a reference to the activity’s **fragment manager** using the activity’s `getFragmentManager()` method. You then use its `findFragmentById()` method to get a reference to the fragment:


![](.guides/img/13.png)

The fragment manager is used to manage any fragments used by the activity. You use it to get references to fragments, and perform fragment transactions. You’ll see more about this later in the chapter.

Here’s our full activity code (replace the existing code in MainActivity.java with the code shown here):

![](.guides/img/14.png)

As you can see, we’ve got a reference to the fragment after calling `setContentView()`. This is really important, because before this, the fragment won’t have been created.

We’re using the code `frag.setWorkout(1)` to tell fragment which workout we want it to display details of. This is the custom method that we created in our fragment. For now, we’re just setting the ID of the workout in the activity’s `onCreate()` method so that we can see some data. Later on, we’ll change it so that the user can select which workout they want to see.

The next thing we need to do is get the fragment to update its views when the fragment is displayed to the user. But before we can do this, we need to understand the fragment’s lifecycle.
