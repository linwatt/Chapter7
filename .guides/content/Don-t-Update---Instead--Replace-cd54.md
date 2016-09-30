Instead of updating the views in `WorkoutDetailFragment`, we will replace it with a new instance of `WorkoutDetailFragment` set up to display details of the next workout that’s been selected. That way, we can store the fragment replacement inside a back stack transaction, and the user will be unable to undo the change by hitting the back button. But how do we replace one fragment with another?


We’ll need to begin by making a change in the *activity_main.xml* layout file. Instead of inserting `WorkoutDetailFragment` directly, we’ll use a **frame layout**.

A **frame layout** is a type of view group that’s used to block out an area on the screen. You define it using the `<FrameLayout>` element. You use it to display single items—in our case, a fragment. We’ll put our fragment in a frame layout so that we can control its contents programmatically. 

Whenever an item in the `WorkoutListFragment` list view gets clicked, we’ll replace the contents of the frame layout with a new instance of `WorkoutDetailFragment` that displays details of the correct workout:

![](.guides/img/41.png)


Add a fragment to an activity using `<fragment>` if you don’t need it to respond to changes in the user interface. Otherwise, use a `<FrameLayout>`.

