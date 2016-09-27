A **list fragment** is type of fragment that specializes in working with a list. It has a default layout that contains the ListView.

![](.guides/img/24.png)

#### Just as with a list activity, there are are a couple of major advantages in using a list fragment to display categories of data:

- **You don’t need to create your own layout**. List fragments define their own layout programmatically, so there’s no XML layout for you to create or maintain. The layout the list fragment generates includes a single list view. You access this list view in your activity code using the list fragment’s `getListView()` method. You need this in order to specify what data should be displayed in the list view.

- **You don’t have to implement your own event listener**. The `ListFragment` class is registered as a listener on the list view, and listens for when items in the list view are clicked. You use the list fragment’s `onListItemClick()` method to get fragment to respond to clicks. You’ll see this in action later on.
