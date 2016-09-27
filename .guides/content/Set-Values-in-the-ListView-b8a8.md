As mentioned in Chapter 6, you can connect data to a list view using an adapter. This is still the case when your list view is in a fragment; ListView is a subclass of the AdapterView class, and it’s this class that allows a view to work with adapters.

We want to supply the list view in `WorkoutListFragment` with an array of workout names, so we’ll use an array adapter to bind the array to the list view.


![](.guides/img/26.png)