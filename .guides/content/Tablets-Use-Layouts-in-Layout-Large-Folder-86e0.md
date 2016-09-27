Getting the tablet version of our app up and running is easy—all we need to do is put our existing activity layout file *activity_main.xml* into the *app/src/main/res/layout-large* folder. The layout in this folder will then only be used by devices with a large screen.


![](.guides/img/62.png)

If the *app/src/main/res/layout-large* folder doesn’t exist in your Android Studio project, you’ll need to create it. To do this, switch to the **Project view** of your folder structure, highlight the *app/src/main/res* folder in the folder explorer, and choose File→New...→Directory. When prompted, give the folder a name of “layout-large”. When you click on the OK button, Android Studio will create the new *app/src/main/res/layout-large* folder for you.

To copy the *activity_main.xml* layout file, highlight the file in the explorer, and choose the Copy command from the Edit menu. Then highlight the new layout-large folder, and choose the Paste command from the Edit menu. Android Studio will copy the *activity_main.xml* file into the *app/src/main/res/layout-large* folder.

If you open the file, it should look like this:

![](.guides/img/63.png)


This layout will be used by devices with a large screen, so when the app is run on a tablet, the two fragments will be displayed side by side. Next, let’s deal with the phone layouts.

