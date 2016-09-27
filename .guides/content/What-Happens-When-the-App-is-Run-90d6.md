**1) When the app is launched, activity MainActivity gets created.**

![](.guides/img/19.png)

**2) MainActivity passes the workout ID to WorkoutDetailFragment in its onCreate() method by calling the fragment’s setWorkout() method.**

![](.guides/img/20.png)

**3) The fragment uses the value of the workout ID in its onStart() method to set the values of its views.**

![](.guides/img/21.png)