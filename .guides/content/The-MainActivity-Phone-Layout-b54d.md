![](.guides/img/64.png)

When the app runs on a phone, we want `MainActivity` to just display `WorkoutListFragment`, and not `WorkoutDetailFragment`. To do this, we’ll update the code in *activity_main.xml* in the *app/src/main/res/layout* folder so that it just contains `WorkoutListFragment`. Any phones that run the app will use the layout in the *layout* folder, whereas any tablets will use the layout in the *layout-large* folder.
