# APK Build Guide for Capacitor

This guide provides step-by-step instructions for building an Android APK using Capacitor.

## Prerequisites
- **Node.js**: Ensure you have Node.js installed (v12 or later recommended).
- **Java Development Kit (JDK)**: Install JDK 8 or later.
- **Android Studio**: Download and install Android Studio and the Android SDK.
- **Gradle**: (Optional) Android Studio should include Gradle, but ensure it is configured properly in SDK Manager.

## Setup Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/davidm24t1y4-ui/https-baffah-companion-ai.lovable.app-auth.git
   cd https-baffah-companion-ai.lovable.app-auth
   ```

2. **Install Capacitor**
   If you haven’t added Capacitor to your project, install it using:
   ```bash
   npm install @capacitor/core @capacitor/cli
   ```

3. **Add Android Platform**
   To add the Android platform to your project:
   ```bash
   npx cap add android
   ```

4. **Sync the Project**
   After making any new changes, sync the project:
   ```bash
   npx cap sync
   ```

## Building Debug APK
1. **Open Android Studio**
   Open the Android folder in Android Studio.

2. **Build APK**
   - Select **Build** from the menu.
   - Click on **Build Bundle(s) / APK(s)** > **Build APK(s)**.
   - Wait for the build to complete, and then find the generated APK in `app/build/outputs/apk/debug`. 

## Building Release APK
1. **Open Android Studio**
   Open the Android project in Android Studio.

2. **Generate Signed APK**
   - Go to **Build** > **Generate Signed Bundle/APK**.
   - Choose **APK** and click **Next**.
   - Select a key store, fill in the credentials, and click **Next**.
   - Select the build variant (usually `release`) and click **Finish**.
   - Find the generated APK in `app/build/outputs/apk/release`.

## Troubleshooting
- Ensure all prerequisites are met. If you encounter build errors, double-check your environment setup.
- If the APK does not run on your device, check the build logs for any runtime errors.
- Make sure your Android Studio is up to date, including all SDK tools.
- You may need to configure additional permissions in the `AndroidManifest.xml` file based on your app's requirements.

## Next Steps
- Test your APK on multiple devices to ensure compatibility.
- Consider signing your app with a release key before uploading to the Play Store.
- Review the [Capacitor Documentation](https://capacitorjs.com/docs) for more advanced configurations and features.

--- 

This guide is up-to-date as of 2026-03-24.