The **back stack** is the list of places that you’ve visited on the device. Each place is a **transaction** on the back stack.

A lot of transactions move you from one activity to another:
```
Transaction: Go to inbox activity
Transaction: Go to 'compose new mail' activity
Transaction: Go to sent mail activity
```

So when you go to a new activity, a transaction to do that is recorded on the back stack. If ever you press the back button, that transaction is reversed, and you’re returned to the activity you were at before.


But back stack transactions don’t have to be activities. They can just be changes to the fragments on the screen:
```
Transaction: Replace the 'Core agony' fragment with 'the wimp special'
```

That means that fragment changes can be undone with the back button, just like activity changes can.
