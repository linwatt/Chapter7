You deal with this problem in a fragment in a similar way to how you deal with it in an activity. You first override the fragment’s `onSaveInstanceState()` method, and put the local variable whose state you want to save in the method’s `Bundle` parameter:

![](.guides/img/51.png)


You then retrieve the value from the `Bundle` in the fragment’s `onCreateView()` method:


![](.guides/img/52.png)