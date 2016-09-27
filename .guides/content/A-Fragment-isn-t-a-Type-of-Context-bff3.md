As you’ve already seen, to create an array adapter that works with a list view, you use: 

![](.guides/img/27.png)

where `DataType` is the type of data, `array` is the array, and `context` is the current context. 

When we used this in an activity, we could use <font style="font-family:courier;">this</font> to get the current context. We could do this because an activity is a type of context—the `Activity` class is a subclass of the `Context` class. 

The Fragment class isn’t a subclass of the Context class, so using `this` won’t work. Instead, you need to get the current context in some other way. If you’re using the adapter in the fragment’s `onCreateView()` method as we are here, you can use the `LayoutInflator` object’s `getContext()` method to get the context instead:

![](.guides/img/28.png)


Once you’ve created the adapter, you bind it to the ListView using the fragment’s `setListAdapter()` method:

![](.guides/img/29.png)

Let’s use an array adapter to populate the list view in our fragment with a list of workouts.