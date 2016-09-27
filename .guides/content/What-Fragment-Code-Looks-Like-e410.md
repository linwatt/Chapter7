The code for the fragment is held in *WorkoutDetailFragment.java* in the app/src/main/java folder. Open this file now.

As you’d expect, Android Studio has generated Java code for you. Replace the code that Android Studio has generated with the code below:

![](.guides/img/9.png)

The above code creates a basic fragment. As you can see, it’s a class that extends `theandroid.app.Fragment` class. All fragments must subclass the `Fragment` class.

Our fragment also implements the `onCreateView()` method. The `onCreateView()`method gets called each time Android needs the fragment’s layout, and it’s where you say which layout the fragment uses. This method is optional, but as you need to implement it whenever you’re creating a fragment with a layout, you’ll need to implement it almost every time you create a fragment.

You specify the fragment’s layout using the code
```
inflater.inflate(R.layout.fragment_workout_detail, container, false);
```
This is the fragment equivalent of an activity’s `setContentView()` method. Just like `setContentView()`, you use it to say what layout the fragment should use. The container argument is passed by the activity that uses the fragment. It’s the `ViewGroup` in the activity that the fragment layout needs to be inserted into.

