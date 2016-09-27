When we created our project, Android Studio created an activity for us called *MainActivity.java*, and a layout called *activity_main.xml*. 
We’re going to change the layout so that it contains the fragment we just created.


![](.guides/img/11.png)
![](.guides/img/10.png)

As you can see, the layout contains one element, <**fragment**>. You use the <**fragment**> element to add a fragment to an activity’s layout. You specify which fragment using the `class` attribute and setting it to the fully qualified name of the fragment. In our case, we’re going to create a fragment called `WorkoutDetailFragment` in the `com.hfad.workout package`, so we use
```
class="com.hfad.workout.WorkoutDetailFragment” 
```

We’ve created a fragment and got the activity to display it in its layout. So far, though, the fragment doesn’t actually do anything. What we need to do next is get the activity to say which workout to display, and get the fragment to populate its views with details of the workout.
