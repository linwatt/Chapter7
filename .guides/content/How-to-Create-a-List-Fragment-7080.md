You add a list fragment to your project in the same way you add a normal fragment. Go to File→New...→Fragment→Fragment (Blank). Give the fragment a name of “WorkoutListFragment”, and then untick the options to create layout XML, and also the options to include fragment factory methods and interface callbacks. 
List fragments define their own layouts programmatically, so you don’t need Android Studio to create one for you. When you click on the Finish button, Android Studio creates a new list fragment for you in a file called *WorkoutListFragment.java* in the app/src/main/java folder.

Here’s what the basic code looks like to create a list fragment. As you can see, it’s very similar to that of a normal fragment. Replace the code in `WorkoutListFragment` with the code below:

![](.guides/img/25.png)

The above code creates a basic list fragment called `WorkoutListFragment`. As it’s a list fragment, it needs to extend the `ListFragment` class rather than `Fragment`.

The `onCreateView()` method is optional. The `onCreateView()` method gets called when the fragment’s view gets created. We’re including it in our code as we want to populate the fragment’s list view with data as soon as it gets created. If you don’t need your code to do anything at this point, you don’t need to include the method.Let’s see how to add data to the list view.
