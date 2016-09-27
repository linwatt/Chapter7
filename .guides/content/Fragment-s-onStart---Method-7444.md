We need to get `WorkoutDetailFragment` to update its views with details of the workout. We need to do this when the activity is started, so we’ll use the fragment’s `onStart()` method. Here’s the code:

![](.guides/img/17.png)

As we said on the previous page, fragments are distinct from activities, and therefore don’t have all the methods that an activity does. Fragments don’t include a `findViewById()` method, for instance. To get a reference to a fragment’s views, we first have to get a reference to the fragment’s root view using the `getView()` method, and use that to find its child views. Now that we’ve got the fragment to update its views, let’s take the app for a test drive. 

You should always call up to the superclass when you implement any fragment lifecycle methods.
