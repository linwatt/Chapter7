- A **fragment** is used to control part of a screen. It can be reused across multiple activities.

- A fragment has an associated layout.

- A fragment is a subclass of the `android.app.Fragment` class.

- The `onCreateView()` method gets called each time Android needs the fragment’s layout.

- Add a fragment to an activity’s layout using the `<fragment>` element and adding a `class` attribute.

- The fragment lifecycle methods tie in with the states of the activity that contains the fragment.

- The `Fragment` class doesn’t extend the `Activity` class or implement the `Context` class.

- Fragments don’t have a `findViewById()` method. Instead, use the `getView()` method to get a reference to the root view, then call the view’s `findViewById()` method.

- A **list fragment** is a fragment that comes complete with a `ListView`. You create one by subclassing `ListFragment`.

- If you need to get a fragment to respond to changes in the user interface, use the `<FrameLayout>` element.

- Use **fragment transactions** to make a set of changes to an existing fragment and add to the **back stack**

- Make apps look different on different devices by putting separate layouts in device-appropriate folders.
