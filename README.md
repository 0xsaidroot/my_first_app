# my_first_app

Lab 1: From zero to a running app on Git.
### Nouredine Ahmad Saïd
### ICTU20241619

## What I learned and what blocked me

### What I learned

I learned how to set up a Flutter development environment. I installed the Flutter SDK, Git, VS Code (with the Flutter extension) and Android Studio (for the Android SDK), and used `flutter doctor -v` to check that each tool was working and to find what was missing.

I learned how to create a Flutter project with `flutter create my_first_app` and how to run it with `flutter run`. I also learned that a Flutter app is built from nested widgets, and that the `build` method describes the screen.

I learned how to use hot reload. After saving a change, or pressing `r` in the terminal, the app updates in about a second without restarting and keeps its state. I used it to change the greeting text, the theme seed colour and the app title, and to add a second `Text` widget in a `Column`.

I learned how to debug the screen size. I used `debugPrint('Screen width: ${MediaQuery.of(context).size.width}')` inside the `build` method and read the value in the debug console.

### What blocked me

The main blocker was my internet connection, which was very slow. Downloading the Android Studio components and the Android virtual device was almost impossible.

Because of this, I could not run the app on my Android phone. The first `flutter run` failed with a Gradle error ("Timeout of 120000 reached waiting for exclusive access to file ... gradle-9.5.0-all.zip"). After retrying, the build failed again because the Android NDK (version 28.2.13676358) could not be downloaded and installed.

I plan to install the NDK when I have a faster connection so that I can run the app on my phone.

I was only able to run the app through chrome

## Screenshots

See the `docs/` folder for the running app and the `flutter doctor` output.