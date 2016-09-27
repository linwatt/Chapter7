### On a Tablet
The tablet version of the app will work in the same way the app does currently:

![](.guides/img/57.png)


### On a phone
Instead of using both fragments inside `MainActivity`, `MainActivity` will use `WorkoutListFragment` and `DetailActivity` will use `WorkoutDetailFragment`. `MainActivity` will start `DetailActivity` when the user clicks on a workout.


![](.guides/img/58.png)

We need to get the app to look and behave differently depending on whether the app is run on a phone or a tablet. To help us do this, let’s see how we can get our app to choose a different layout depending on the type of device it’s running on.