We’re going to add a new fragment called `WorkoutDetailFragment` to the project to display details of a single workout. You add a new fragment in a similar way to how you add a new activity. In Android Studio, go to File→New...→Fragment→Fragment (Blank).

You will be asked to choose options for your new fragment. Give the fragment a name of “WorkoutDetailFragment”, tick the option to create layout XML for it, and give the fragment layout a name of “fragment_workout_detail”. 

Untick the options to include fragment factory methods and interface callbacks; these options generate extra code which you don’t need to use. When you’re done, click on the Finish button.

![](.guides/img/7.png)


When you click on the Finish button, Android Studio creates a new fragment file called WorkoutDetailFragment.java in the app/src/main/java folder, and a new layout file called fragment_workout_detail.xml in the app/src/res/layout folder.