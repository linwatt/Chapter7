**Fragments** are like reusable components or subactivities. A fragment is used to control part of a screen, and can be reused between screens. This means we can create a fragment for the list of workouts, and a fragment to display the details of a single workout. These fragments can then be shared between layouts.


![](.guides/img/3.png)

Just like an activity, a fragment has an associated layout. If you design it carefully, the Java code can be used to control everything within the interface. If the fragment code contains all that you need to control its layout, it greatly increases the chances that you’ll be able to reuse it elsewhere in the app. We’re going to show you how to create and use fragments by building the Workout app.
