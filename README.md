# AndroidDependencies
It is an Android module which contains base dependencies for creating an app

- Add below lines at the build.gradle inside app module.

```
apply plugin: "kotlin-kapt"
apply from: './dependencies.gradle'
```

## Appcompat
[latest version](https://developer.android.com/jetpack/androidx/releases/appcompat)

```
def appcompat_version = "1.1.0"
implementation "androidx.appcompat:appcompat:$appcompat_version"
```

## Constraintlayout
[latest version](https://developer.android.com/jetpack/androidx/releases/constraintlayout)

```
def constraintlayout_version = ""
implementation "androidx.constraintlayout:constraintlayout:$constraintlayout_version"
```

## Core
[latest version](https://developer.android.com/jetpack/androidx/releases/core)
```
def core_version = ""
implementation "androidx.core:core-ktx:$core_version"
```

## Fragment
[latest version](https://developer.android.com/jetpack/androidx/releases/fragment)
```
def fragment_version = ""
implementation "androidx.fragment:fragment-ktx:$fragment_version"
// Testing Fragments in Isolation
implementation "androidx.fragment:fragment-testing:$fragment_version"
```

## Lifecycle
[latest version](https://developer.android.com/jetpack/androidx/releases/lifecycle)
```
def lifecycle_version = ""

implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-livedata-ktx:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-runtime-ktx:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-viewmodel-savedstate:$lifecycle_version"
kapt "androidx.lifecycle:lifecycle-compiler:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-common-java8:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-service:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-process:$lifecycle_version"
implementation "androidx.lifecycle:lifecycle-reactivestreams-ktx:$lifecycle_version"
testImplementation "androidx.arch.core:core-testing:$arch_version"
```

## Navigation
 [latest version](https://developer.android.com/jetpack/androidx/releases/navigation)

```
def nav_version = ""

implementation "androidx.navigation:navigation-fragment-ktx:$nav_version"
implementation "androidx.navigation:navigation-ui-ktx:$nav_version"

// Testing Navigation
androidTestImplementation "androidx.navigation:navigation-testing:$nav_version"
```

## Room
[latest version](https://developer.android.com/jetpack/androidx/releases/room)
```
def room_version = ""

implementation "androidx.room:room-runtime:$room_version"
annotationProcessor "androidx.room:room-compiler:$room_version" // For Kotlin use kapt instead of annotationProcessor

// optional - Kotlin Extensions and Coroutines support for Room
implementation "androidx.room:room-ktx:$room_version"

// optional - RxJava support for Room
implementation "androidx.room:room-rxjava2:$room_version"

// optional - Guava support for Room, including Optional and ListenableFuture
implementation "androidx.room:room-guava:$room_version"

// Test helpers
testImplementation "androidx.room:room-testing:$room_version"
```

## WorkManager
[latest version](https://developer.android.com/jetpack/androidx/releases/work)
```
def work_version = ""

// Kotlin + coroutines
implementation "androidx.work:work-runtime-ktx:$work_version"

// optional - RxJava2 support
implementation "androidx.work:work-rxjava2:$work_version"

// optional - GCMNetworkManager support
implementation "androidx.work:work-gcm:$work_version"

// optional - Test helpers
androidTestImplementation "androidx.work:work-testing:$work_version"
```

## Retrofit
[latest version](https://github.com/square/retrofit/releases)
```
def retrofit_version = ""
implementation "com.squareup.retrofit2:retrofit:$retrofit_version"
implementation "com.squareup.retrofit2:converter-moshi:$retrofit_version"
implementation "com.squareup.retrofit2:converter-gson:$retrofit_version"
```

## Logging Interceptor
[latest version](https://github.com/square/okhttp/tree/master/okhttp-logging-interceptor)

```
def loggin_interceptor = "4.5.0"
implementation("com.squareup.okhttp3:logging-interceptor:$loggin_interceptor")
```

## Moshi
[latest version](https://github.com/square/moshi/releases)
```
def moshi_version = ""
implementation "com.squareup.moshi:moshi-kotlin:$moshi_version"
kapt "com.squareup.moshi:moshi-kotlin-codegen:$moshi_version"
```

## Coroutine
[latest version](https://github.com/Kotlin/kotlinx.coroutines/releases)

```
def coroutines_version = ""
implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:$coroutines_version"
implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:$coroutines_version"
```

## RxAndroid
[latest_version](https://github.com/ReactiveX/RxAndroid/releases)

```
def rx_version = "3.0.0"
implementation "io.reactivex.rxjava3:rxandroid:$rx_version"
implementation "io.reactivex.rxjava3:rxjava:$rx_version"
implementation "io.reactivex.rxjava3:rxkotlin:$rx_version"
```

## Material Components for Android
[latest version](https://mvnrepository.com/artifact/com.google.android.material/material)
```
def material_version = ""
implementation "com.google.android.material:material:$material_version"
```

## Dagger
[latest_version](https://github.com/google/dagger/releases)

```
def dagger_version = "2.27"
api "com.google.dagger:dagger:$dagger_version"
kapt "com.google.dagger:dagger-compiler:$dagger_version"
api "com.google.dagger:dagger-android:$dagger_version"
api "com.google.dagger:dagger-android-support:$dagger_version" 
kapt "com.google.dagger:dagger-android-processor:$dagger_version"
```

## Timber
[latest_version](https://github.com/JakeWharton/timber/releases)

```
def timber_version = ""
implementation "com.jakewharton.timber:timber:$timber_version"
```

## Koin
[latest version](https://github.com/InsertKoinIO/koin/releases)

```
def koin_version = '2.1.5'
implementation "org.koin:koin-android:$koin_version"
// Koin AndroidX Scope features
implementation "org.koin:koin-androidx-scope:$koin_version"
// Koin AndroidX ViewModel features
implementation "org.koin:koin-androidx-viewmodel:$koin_version"
// Koin AndroidX Fragment features
implementation "org.koin:koin-androidx-fragment:$koin_version"
// Koin AndroidX Experimental features
implementation "org.koin:koin-androidx-ext:$koin_version"
```

## Anko
[latest version](https://github.com/Kotlin/anko/releases)

```
def anko_version = '0.10.8'
implementation "org.jetbrains.anko:anko:$anko_version"
```


## Gson
[latest version](https://github.com/google/gson/releases)

```
def gson_version = '2.8.6'
implementation "com.google.code.gson:gson:$gson_version"
```

## LeakCanary
[latest version](https://square.github.io/leakcanary/changelog/)

```

def leakcanary_version = '2.2'
debugImplementation "com.squareup.leakcanary:leakcanary-android:$leakcanary_version"
```
