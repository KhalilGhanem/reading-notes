# Intent Filters

An Intent is a messaging object you can use to request an action from another app component.

Intents facilitate communication between components in several ways, there are three fundamental use cases:

* Starting an activity
* Starting a service
* Delivering a broadcast

## Intent Filter

An intent filter is an expression in an app's manifest file that specifies the type of intents that the component would like to receive.

## Allowing Other Apps to Start Your Activity

If our app can perform an action that might be useful from another app, we should make our app be prepared to respond to action requests by specifying the appropriate intent filter in our activity.

To allow other apps to start our activity , we need to add an `<intent-filter>` element in our manifest file for the corresponding `<activity>` element.

## Add an Intent Filter

In order to properly define which intents our activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.

The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

* Action: A string naming the action to perform. Usually one of the platform-defined values such as `ACTION_SEND` or `ACTION_VIEW`.
* Data: A description of the data associated with the intent.
* Category: Provides an additional way to characterize the activity handling the intent.

## Handle the Intent in Your Activity

As your activity starts, call getIntent() to retrieve the Intent that started the activity.

## Return a Result

We should call `setResult()` to specify the result code and result Intent.
