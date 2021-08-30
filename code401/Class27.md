# Intents, Activities, and SharedPreferences

## Understand Tasks and Back Stack
* A task is a collection of activities that users interact with when performing a certain job. 
* The activities are arranged in a stack—the back stack)—in the order in which each activity is opened.
* When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface.
* When the user presses the Back button, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes.
* Activities in the stack are never rearranged, only pushed and popped from the stack.
* Because the activities in the back stack are never rearranged, if your app allows users to start a particular activity from more than one activity, a new instance of that activity is created and pushed onto the stack.

## Managing Tasks
We managing tasks to interrupt the normal behavior of the back stack.

We can do this with  attributes in the `<activity>` manifest element and with flags in the intent that you pass to startActivity().

In this regard, the principal`<activity>` attributes you can use are:
* taskAffinity
* launchMode
* allowTaskReparenting
* clearTaskOnLaunch
* alwaysRetainTaskState
* finishOnTaskLaunch

And the principal intent flags you can use are:
* FLAG_ACTIVITY_NEW_TASK
* FLAG_ACTIVITY_CLEAR_TOP
* FLAG_ACTIVITY_SINGLE_TOP

## Save key-value data
We used the SharedPreferences APIs to save a relatively small collection of key-values.

A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them.

Each SharedPreferences file is managed by the framework and can be private or shared.

You can create a new shared preference file or access an existing one by calling one of these methods:

* getSharedPreferences() — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter.
* getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity.