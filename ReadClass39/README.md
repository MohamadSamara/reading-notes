# Read Class 39

**What are the benefits and downfalls of using the ‘getLastLocation()’ method to get your device’s location?**

The `getLastLocation()` method retrieves the most recent location update that has been recorded by the device. This method is useful if you only need the device's location for a single purpose and do not need real-time updates.

**Benefits:**

* **Quick and efficient:** `getLastLocation()` is typically faster than `getCurrentLocation()` because it does not need to request a new update from the location providers.
* **Minimizes battery usage:** `getLastLocation()` does not require the device to continuously update its location, which can save battery life.

**Drawbacks:**

* **Accuracy:** The last known location may not be the device's current location, especially if the device has been stationary for a while.
* **Stale data:** The last known location may not be up-to-date if the device has been offline or if the location providers have not been able to get a fix.

**What about the ‘getCurrentLocation()’ method?**

The `getCurrentLocation()` method requests a new location update from the device's location providers. This method is useful if you need the device's most up-to-date location, such as for real-time tracking or navigation.

**Benefits:**

* **Accuracy:** `getCurrentLocation()` typically returns the most up-to-date location information available.
* **Real-time updates:** `getCurrentLocation()` can be used to subscribe to real-time location updates, which allows you to track the device's location as it moves.

**Drawbacks:**

* **Slower:** `getCurrentLocation()` may be slower than `getLastLocation()` because it needs to request a new update from the location providers.
* **More power consumption:** `getCurrentLocation()` can consume more battery power than `getLastLocation()` because it requires the device to continuously update its location.
