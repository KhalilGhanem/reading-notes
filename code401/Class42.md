# Location

## Request location permissions

To protect user privacy, apps that use location services must request location permissions.

The Android system includes multiple permissions related to location. Which permissions you request, and how you request them, depend on the location requirements for your app's use case.

## Types of location access

Android's location permissions deal with the following categories of location access:

### 1-Foreground location:

foreground location access is when our app shares or receives location information only once, or for a defined amount of time.

The system considers your app to be using foreground location if a feature of your app accesses the device's current location in one of the following situations:

* An activity that belongs to your app is visible.
* When the app is running a foreground service.

On Android 10 (API level 29) and higher, we must declare the foreground service type

``` ex
    Example:
    <service
        android:name="MyNavigationService"
        android:foregroundServiceType="location" ... >
        <!-- Any inner elements would go here. -->
    </service>
```

We need to declare a  foreground location when our app requests either the ACCESS_COARSE_LOCATION permission or the ACCESS_FINE_LOCATION permission like the example follow:

```ex
    Example
    <manifest ... >
    <!-- To request foreground location access, declare one of these permissions. -->
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
    </manifest>
```

The level of precision depends on which permission we request:

* `ACCESS_COARSE_LOCATION`: Provides an estimate of the device's location, to within about 1 mile (1.6 km).
* `ACCESS_FINE_LOCATION` : Provides an estimate of the device's location that is as accurate as possible, usually within about 160 feet (50 meters) and sometimes as accurate as within 10 feet (a few meters) or better.

### 2-Background location:

background location accessis when our app shares or receives location information constantly

On Android 10 (API level 29) and higher, we must declare the ACCESS_BACKGROUND_LOCATION permission in our app's manifest in order to request background location access at runtime.

```ex
    <manifest ... >
    <!-- Required only when requesting background location access on
        Android 10 (API level 29) and higher. -->
    <uses-permission android:name="android.permission.ACCESS_BACKGROUND_LOCATION" />
    </manifest>
```

## Get the last known location

Our app can request the last known location of the user's device, by using the Google Play services location APIs.

We will use the `fused location provider` to retrieve the device's last known location.

The fused location provider is one of the location APIs in Google Play services. It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level, like high accuracy or low power.

## how to make a single request for the location of a device using the getLastLocation() method in the fused location provider:

* Set up Google Play services
  
  To access the fused location provider, our app's development project must include Google Play services. Download and install the Google Play services component via the SDK Manager and add the library to your project.
* Specify app permissions

  Apps whose features use location services must request location permissions, depending on the use cases of those features.  
* Create location services client
  
  * In our activity's onCreate() method, create an instance of the Fused Location Provider Client as the following code
    ```
            private FusedLocationProviderClient fusedLocationClient;

        // ..

        @Override
        protected void onCreate(Bundle savedInstanceState) {
            // ...

            fusedLocationClient = LocationServices.getFusedLocationProviderClient(this);
        }
    ```
* Get the last known location: We will use `getLastLocation()` method to retrieve the device location.
* Choose the best location estimate

  The FusedLocationProviderClient provides several methods to retrieve device location information.

  * `getLastLocation()` gets a location estimate more quickly and minimizes battery usage that can be attributed to our app.
  * `getCurrentLocation()` gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device.
  