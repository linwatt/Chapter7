We have two objects that need to talk to each other—the fragment and the activity—and we want them to talk without one side knowing too much about the other. So we don’t have to duplicate the code for each fragment. The way we do that in Java is with an **interface**. When we define an interface, we’re saying what the minimum requirements are for one object to talk usefully to another. It means that we’ll be able to get the fragment to talk to any kind of activity, so long as that activity implements the interface.

We’re going to create an interface called `WorkoutListListener`, that looks like this:

![](.guides/img/36.png)

So long as an activity implements this interface, we’ll be able to tell it that an item on the list fragment has been clicked. This is what will happen at runtime:

**1)** The `WorkoutListListener` will tell the fragment that it wants to listen.

**2)** A user will click on a workout in the list.

**3)** The `onListItemClicked()` method in the list-fragment will be called.

**4)** That method will then call the `WorkoutListListener`’s `itemClicked()` method with the ID of the workout that was clicked
