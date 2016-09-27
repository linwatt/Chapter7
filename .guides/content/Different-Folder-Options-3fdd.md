You can put all kinds of resources (drawables or images, layouts, menus, and values) in different folders to specify which types of device they should be used with. The screen-specific folder name can include screen size, density, orientation and aspect ratio, each part separated by hyphens.

As an example, if you want to create a layout that will only be used by very large tablets in landscape mode, you would create a folder called layout-xlarge-land and put the layout file in that folder. Here are the different options you can use for the folder names:


![](.guides/img/60.png)

Android decides at runtime which resources to use by looking for the best match. If there’s no exact match, it will use resources designed for a smaller screen than the current one. If resources are only available for screens larger than the current one, Android won’t use them and the app will crash.

If you only want your app to work on devices with particular screen sizes, you can specify this in *AndroidManifest.xml* using the `<supports-screens>` attribute. As an example, if you don’t want your app to run on devices with small screens, you’d use

![](.guides/img/61.png)

Using the different folder names, you can create layouts that are specific for phones and tablets. 

For more info on screens and layouts, visit the [Android Developer](https://developer.android.com/guide/practices/screens_support.html) site.