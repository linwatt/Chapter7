You replace the fragment at runtime inside a **fragment transaction**. A fragment transaction is a set of changes you want to apply relating to the fragment, all at the same time. 

To create a fragment transaction, you start by getting a `FragmentTransaction` from the fragment manager:

![](.guides/img/42.png)

You then specify all the actions you want to group together in the transaction. In our case, we want to replace the fragment in the frame layout, and we do this using the fragment’s `replace()` method:

![](.guides/img/43.png)

where `R.id.fragment_container` is the ID of the container containing the fragment. You may also add a fragment to a container using the `add()` method, or remove a fragment using the `remove()` method:

![](.guides/img/44.png)

You can use the `setTransition()` method to say what sort of transition animation you want for this transaction.

![](.guides/img/45.png)
where `transition` is the type of animation. Options for this are `TRANSIT_FRAGMENT_CLOSE` (a fragment is being removed from the stack), `TRANSIT_FRAGMENT_OPEN` (a fragment is being added), `TRANSIT_FRAGMENT_FADE` (the fragment should fade in and out) and `TRANSIT_NONE` (no animation).

Once you’ve specified all the actions you want to take as part of the transaction, you can use the `addToBackStack()` method to add the transaction to the back stack of transactions. This allows the user to go back to a previous state of the fragment when they press the Back button. The `addToBackStack()` method takes one parameter, a String name you can use to label the transaction:

![](.guides/img/46.png)

To commit the changes to the activity, you call the `commit()` method:

![](.guides/img/47.png)

The `commit()` method applies the changes.

