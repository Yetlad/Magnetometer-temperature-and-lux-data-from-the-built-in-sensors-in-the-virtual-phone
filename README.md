
## Sensor App 

##  Overview
This project is an Android application built with **Kotlin** and **Jetpack Compose** that reads data from device sensors and displays them in real time.  
The app demonstrates:
- Accessing hardware sensors via **SensorManager**.  
- Managing sensor data with **ViewModel** and **StateFlow**.  
- Persisting user preferences (font style) using **DataStore**.  
- Displaying sensor values in a Compose UI with selectable font styles.


## Features
- **Magnetometer** → Displays X, Y, Z axis values.  
- **Ambient Temperature** → Displays current temperature (if supported by device).  
- **Light Sensor** → Displays lux values.  
- **Font Style Preference** → User can choose between *Default*, *Bold*, or *Italic*. Preference is saved with **DataStore** and restored on next launch.  

## Tech Stack
- **Kotlin**  
- **Jetpack Compose**  
- **Android ViewModel + StateFlow**  
- **SensorManager API**  
- **DataStore Preferences**  



## Dependencies
Add the following in **build.gradle.kts (Module: app)**:

```kotlin
dependencies {
    implementation("androidx.lifecycle:lifecycle-runtime-ktx:2.6.2")
    implementation("androidx.lifecycle:lifecycle-viewmodel-compose:2.6.2")
    implementation("androidx.datastore:datastore-preferences:1.0.0")
}
```

---

## Example Output
```
Magnetometer: X: -12.34, Y: 45.67, Z: 89.01
Temperature: 25.0 ℃
Light (Lux): 36.0
Font Style: Bold
```

---

## Conclusion
This app demonstrates how to integrate **hardware sensors** with **Jetpack Compose** and manage persistent user preferences using **DataStore**. It fulfills the assignment requirements by reading sensor data, displaying it in a reactive UI, and allowing customization of font styles.

