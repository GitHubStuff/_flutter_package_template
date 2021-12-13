# empty_package

This is a template kit (with example) to create a Flutter Package.

The template project is a good foundation for creating packages that uses with BLoC and Modular programming patterns.

## Setup

- After un-ziping, rename the folder from _template_package to "new name"

- Open the project in IDE of choice and search/replace "empty_package" with "new package name". This 100% works using VSCode.

- Rename 'empty_package.dart' to the "new package name" (eg custom_widget_package.dart)

- Search/Replace 'com.replace_domain' to your reverse-domain

- Localization: At the root of the template is **/l10n**, within are **.arb** files with the localization key/value pairs. On **flutter pub get** the localization files will be generated in both the *packge* AND */example* space. There are **mixin.dart** files in both spaces that provide a **lookup** mixin, that uses the vales of **dictionary_emum** to get localized text

- Begin coding.

### Note

In the /example folder is a skeleton app that has ThemeManager defined, as well as sample screen that has a dark/light mode option built in the top-left corner. This always for dark/light mode testing as package is being tested.

## Useage

The 'example' directory is an app that includes:

- Usage of [flutter_block](https://pub.dev/packages/flutter_bloc)

- Usage of [flutter_modular](https://pub.dev/packages/flutter_modular)

- Localizations using [intl](https://pub.dev/packages/intl)

- User settable Light/Dark mode using [ThemeManager](https://github.com/GitHubStuff/theme_manager) {Tap the light-bulb in the upper right corner}

## Final note

Be kind to each other!
