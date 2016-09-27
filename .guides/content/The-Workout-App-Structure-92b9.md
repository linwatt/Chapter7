Here’s a breakdown of how the app is structured, and what it does:

![](.guides/img/4.png)

**1) When the app gets launched, it starts activity MainActivity.**
The activity uses layout activity_main.xml.

**2) The activity uses two fragments, WorkoutListFragment, and WorkoutDetailFragment.**

**3) WorkoutListFragment displays a list of workouts.**
It uses *fragment_workout_list.xml* as its layout.

**4) WorkoutDetailFragment displays details of a workout.**
It uses *fragment_workout_detail.xml* as its layout.

**5) Both fragments get their workout data from Workout.java.**
*Workout.java* contains an array of `Workouts`.
