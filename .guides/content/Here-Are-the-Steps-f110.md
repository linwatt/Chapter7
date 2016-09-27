There are a number of steps we’ll go through to build the app:

![](.guides/img/5.png)

**1) Create the fragments.**
We’ll create two fragments. `WorkoutListFragment` will be used to display a list of workouts, and `WorkoutDetailFragment` will be used to display details of a specific workout. We’ll display these fragments in a single activity. We’ll also add a plain old Java Workout class that the fragments will use to get their data from.

**2) Link the two fragments.**
When we click on a workout in `WorkoutListFragment`, we want to display details of the workout in `WorkoutDetailFragment`.

**3) Create device-specific layouts.**
Finally, we’re going to change our app so that it looks and behaves differently depending on what sort of device it’s run on. If it’s run on a device with a large screen, the fragments will be displayed alongside each other. If not, they’ll be displayed in separate activities.
