Earlier in the book, you saw how you could get different devices to use image resources appropriate to their screen size by putting different sized images in the different drawable folders. As an example, you put images you want devices with high density screens to use in the drawable-hdpi folder.

You can do something similar with other resources such as layouts, menus, and values. If you want to create multiple versions of the same resources for different screen specs, you just need to create multiple resource folders with an appropriate name. The device will then load the resources at runtime from the folder that’s the closest match to its screen spec.

As an example, if you want to have one layout for large screen devices, and a couple of other layouts for other devices, you put the layout for the large device in the *app/src/main/res/layout-large folder*, and the layouts for the other devices in the *app/src/main/res/layout* folder. When the app gets run on a device with a large screen, the device will use the layout in the layout-large folder:


![](.guides/img/59.png)