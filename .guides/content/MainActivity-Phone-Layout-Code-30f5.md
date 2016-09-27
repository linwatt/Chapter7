
To do this, open the *activity_main.xml* file in the *app/src/main/res/layout* folder, then replace the XML with the code below:

![](.guides/img/65.png)

As `MainActivity` only needs to display `WorkoutListFragment` when it’s running on a phone, there’s no need for us to create a separate layout that contains the `<fragment>` element. This is only necessary when you need to display multiple fragments.

Note that the version of *activity_main.xml* in the *layout* folder doesn’t contain the `fragment_container` frame layout, whereas the version of *activity_main.xml* in the *layout-large* folder does. This is because only the version of *activity_main.xml* in the *layout-large* folder needs to display `WorkoutDetailFragment`. Later on, we’ll be able to use this fact to figure out which layout the app’s using on the user’s device.

Next, we need to create a second activity that uses `WorkoutDetailFragment`.