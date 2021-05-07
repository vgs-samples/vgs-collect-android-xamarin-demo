[![license](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/verygoodsecurity/vgs-collect-android/blob/master/LICENSE)

# VGS Collect SDK. Xamarin Demo.
Binding library for VGS Collect Android SDK


> **_NOTE:_**  This demo is just an example of how VGS Collect SDK can be integrated into your application.

## How to run it?

### Step 1

Go to your <a href="https://dashboard.verygoodsecurity.com/" target="_blank">VGS organization</a> and establish <a href="https://www.verygoodsecurity.com/docs/getting-started/quick-integration#securing-inbound-connection" target="_blank">Inbound connection</a>. For this demo you can import pre-built route configuration:

<p align="center">
<img src="images/dashboard_routs.png" width="600">
</p>

- Find the **configuration.yaml** file inside the app repository and download it.
- Go to the **Routes** section on the <a href="https://dashboard.verygoodsecurity.com/" target="_blank">Dashboard</a> page and select the **Inbound** tab.
- Press **Manage** button at the right corner and select **Import YAML file**.
- Choose **configuration.yaml** file that you just downloaded and tap on **Save** button to save the route.

### Step 2

`git clone git@github.com:vgs-samples/vgs-collect-android-xamarin-demo.git`

### Step 3

* <b>VGSCollectBindingLibrary</b> - Android Binding Library
* <b>AndroidSample</b> - Sample of the Xamarin Android project with VGS collect library integrated

#### Dependencies

**VGSCollectBindingLibrary**
* Xamarin.Kotlin.StdLib 1.3.50.1
* Xamarin.AndroidX.AppCompat 1.1.0
* Square.OkHttp3 4.2.2
* Xamarin.Kotlin.StdLib.Jdk8 1.3.50.1

**AndroidSample**
* Xamarin.Android.Support.Design 28.0.0.3
* Xamarin.AndroidX.AppCompat 1.1.0
* Xamarin.AndroidX.Legacy.Support.Core.UI 1.0.0
* Xamarin.AndroidX.Lifecycle.LiveData 2.2.0
* Xamarin.Google.Android.Material 1.1.0-rc3
* Xamarin.Kotlin.StdLib 1.3.50.1
* Xamarin.Android.Support.Annotations 28.0.0.3
* Square.OkHttp3 4.2.2
* Xamarin.Kotlin.StdLib.Jdk8 1.3.50.1


### Step 4

Setup `"<VAULT_ID>"`.

**VGS Collect SDK**. Find [MainActivity.cs](https://github.com/vgs-samples/vgs-collect-android-xamarin-demo/blob/master/AndroidSample/MainActivity.cs#L27) and replace `VAULT_ID` constant with your <a href="https://www.verygoodsecurity.com/docs/terminology/nomenclature#vault" target="_blank">vault id</a>.


### Step 5

How to integrate compiled library
1. In the target Xamarin Android project right click on References
2. Add Reference
3. Switch to .Net Assembly tab
4. Choose compiled dll from the file system


### Step 6

1. Open Visual Studio
2. Choose configuration
3. Run build
4. It may be needed to install required Android SDK

Compiled library Build also available under <b>{Project_root}/dll</b> folder


### Step 7

Submit and reveal the form then go to the Logs tab on a Dashboard find a request and secure a payload.
Instruction for this step you can find <a href="https://www.verygoodsecurity.com/docs/getting-started/quick-integration#securing-inbound-connection" target="_blank">here</a>.

## License
VGS Collect Android SDK is released under the MIT license. [See LICENSE](https://github.com/verygoodsecurity/vgs-collect-android/blob/master/LICENSE) for details.
