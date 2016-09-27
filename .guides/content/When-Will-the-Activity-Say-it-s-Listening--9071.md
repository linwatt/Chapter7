When will the activity tell the fragment that it’s ready to receive updates about what item’s been clicked? If you look back at the fragment lifecycle, you’ll see that when the fragment is attached to the activity, the fragment’s `onAttach()` method is called with the value of the activity:

![](.guides/img/37.png)

We can use this method to register the activity with the fragment. 
