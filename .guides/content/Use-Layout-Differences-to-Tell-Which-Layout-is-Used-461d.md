We want `MainActivity` to perform different actions when the user clicks on a workout depending on whether the device is using *activity_main.xml* in the *layout* or *layout-large* folder.

If the app is running on a phone, the device will be using *activity_main.xml* in the *layout* folder. This layout doesn’t include `WorkoutDetailFragment`, so if the user clicks on a workout, we want `MainActivity` to start `DetailActivity`.

![](.guides/img/70.png)

If the app is running on a tablet, the device will be using *activity_main.xml* in the *layout-large* folder. This layout includes a frame layout with an ID of `fragment_container` that’s used to display `WorkoutDetailFragment`. If the user clicks on a workout in this case, we need to display a new instance of `WorkoutDetailFragment` in the `fragment_container` frame layout.

![](.guides/img/71.png)

We can deal with both these situations in `MainActivity` by checking which layout the device is using. We can tell this by looking for a view with an ID of `fragment_container`.

If `fragment_container` exists, the device must be using *activity_main.xml* in the *layout-large* folder, so we know we have to display a new instance of `WorkoutDetailFragment` when the user clicks on a workout. If `fragment_container` doesn’t exist, the device must be using the version of *activity_main.xml* in the *layout* folder, so we need to start `DetailActivity` instead.
