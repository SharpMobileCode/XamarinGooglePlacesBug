# XamarinGooglePlacesBug

## Description
When adding a reference to the [Xamarin.Google.Android.Places](https://www.nuget.org/packages/Xamarin.Google.Android.Places/1.1.0.1) Nuget Package (version 1.1.0.1), I get the following compile error on my Android application:

```
/MyUserPath/XamarinGooglePlacesBug/XamarinGooglePlacesBug/obj/Debug/android/src/mono/com/android/volley/Request_NetworkRequestCompleteListenerImplementor.java(29,29): Error:  error: NetworkRequestCompleteListener is not public in Request; cannot be accessed from outside package
		com.android.volley.Request.NetworkRequestCompleteListener
 (XamarinGooglePlacesBug)
```

## Steps To Reproduce
1. Clone the repo at [https://github.com/SharpMobileCode/XamarinGooglePlacesBug](https://github.com/SharpMobileCode/XamarinGooglePlacesBug)
2. Compile the Android application.

## Expected Result
The android application should compile without error and the Android Google Places SDK should be available to use.

## Actual Result
The android application produces an a compile error:
```
/MyUserPath/XamarinGooglePlacesBug/XamarinGooglePlacesBug/obj/Debug/android/src/mono/com/android/volley/Request_NetworkRequestCompleteListenerImplementor.java(29,29): Error:  error: NetworkRequestCompleteListener is not public in Request; cannot be accessed from outside package
		com.android.volley.Request.NetworkRequestCompleteListener
 (XamarinGooglePlacesBug)
```
