Now we need to make *MainActivity.java* implement the `WorkoutListListener` interface we just created. Update your code to match:


![](.guides/img/39.png)

When an item is clicked in the fragment, the `itemClicked()` method in the activity will be called. We can put code in this method to show the details of the workout that’s just been selected.

#### But how do we update the workout details?
The `WorkoutDetailFragment` updates its views when the fragment is started. But once it's displayed on screen, how do we get it to update the details?

You might think we could play with the fragment's lifecycle so that we can get it to update. Instead, **we'll replace the detail fragment with a brand-new detail fragment, each time we want its text to change.**

### Why?
