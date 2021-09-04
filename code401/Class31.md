# Espresso

Espresso a testing framework designed to provide a fluent API for writing concise and reliable UI tests. 

We Use Espresso to write concise, beautiful, and reliable Android UI tests.
```R
Espresso test example:
@Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("Steve"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}
```

**Espresso tests run optimally fast! It lets you leave your waits, syncs, sleeps, and polls behind while it manipulates and asserts on the application UI when it is at rest.**

## Target audience

Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle.

## Synchronization capabilities

Each time your test invokes onView(), Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:

* The message queue is empty.
* There are no instances of AsyncTask currently executing a task.
* All developer-defined idling resources are idle.

## Create UI tests with Espresso Test Recorder 

The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code. By recording a test scenario.

### Record an Espresso test

Espresso tests consist of two primary components:

* UI interactions: include tap and type actions that a person may use to interact with your app.
* assertions on View elements: verify the existence or contents of visual elements on the screen.

### Record UI interactions

1. Click Run > Record Espresso Test.
2. In the Select Deployment Target window, choose the device on which you want to record the test. 
3. The Record Your Test window appears after the app launches.

### Add assertions to verify UI elements

Assertions verify the existence or contents of a View element through three main types:

* text is: Checks the text content of the selected View element
* exists: Checks that the View element is present in the current View hierarchy visible on the screen
* does not exist: Checks that the View element is not present in the current View hierarchy

**To add an assertion to the test:**

1. Click Add Assertion.
2. To select a View element on which to create an assertion, click on the element in the screenshot or use the first drop-down menu in the Edit assertion box at the bottom of the window.
3. Select the assertion you want to use from the second drop-down menu in the Edit assertion box.
4. Click Save Assertion to close the assertion panels.
