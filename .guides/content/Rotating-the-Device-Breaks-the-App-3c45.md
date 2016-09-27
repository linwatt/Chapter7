When you rotate the app, there’s a problem. Regardless of which workout you’ve chosen, when you rotate the device, the app displays details of the first workout.


![](.guides/img/50.png)

When we first looked at the activity lifecycle, you saw how when you rotate the device, Android destroys and re-creates the activity. When this happens, local variables used by the activity can get lost. If the activity uses a fragment, **the fragment gets destroyed and re-created along with the activity**. This means that any local variables used by the fragment can also lose their state.

In our `WorkoutDetailFragment`, we use a local variable called `workoutId` to store the ID of the workout the user clicks on in the `WorkoutListFragment` list view. When the user rotates the device, `workoutId` loses its current value and it’s set to 0 by default. The fragment then displays details of the workout with an ID of 0—the first workout in the list.


