The layout just needs to contain the fragment `WorkoutDetailFragment`. Update the code in *activity_detail.xml* as follows:


![](.guides/img/67.png)

As well as updating the *activity_detail* layout, we need to update `DetailActivity` itself. If the app is running on a phone, `MainActivity` will need to start `DetailActivity` using an intent. This intent will need to include the ID of the workout the user has selected as extra information. The `DetailActivity` will then need to pass this to the `WorkoutDetailFragment` using its `setWorkout()` method.

![](.guides/img/68.png)
