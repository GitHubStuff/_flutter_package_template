# empty_package

This is a template kit (with */example*) to create a Flutter Package.

The template project is a great foundation for creating packages that uses with BLoC and Modular programming patterns.

The package also contains an ad-hoc */example* folder with an app designed to load the new package and quickly allow the developer to create a demo/POC/beta-sample.

**^^The */example* that creates an app is also a great foundation for an app beyond development and proof-of-concept(POC)**

---

## Setup

### Changes to content of template

- After un-ziping, rename the folder from _template_package to "new name"

- Rename 'lib/*empty_package.dart*' to the "new package name" (eg custom_widget_package.dart)

- Open the project in IDE of choice and search/replace "*empty_package*" with "new package name". This 100% works using VSCode.

- Search/Replace '*replace_domain*' with project/company domain.

#### NOTE

***replace_domain** will be part of the reverse domain used by XCode and Android in the app/product name. Choose carefully!*

### Optional action for **localization**

- [Optional] Search/Replace '*DictionaryEnum*' with a name better suited for your app's vocabulary

- Localization: At the root of the template is **/l10n**, within are **.arb** files with the localization key/value pairs. On **flutter pub get** the localization files will be generated in both the *packge* AND */example* space. There are **mixin.dart** files in both spaces that provide a **lookup** mixin, that uses the vales of ***DictionaryEnum*** to get localized text

### **Important**: Make these ***Setup*** changes your initial comment to version control before proceeding

&nbsp;
&nbsp;

---
&nbsp;

## After setup & commit to version control

- Review and update the *README-template.md*

- Delete the *README.md*

- Rename *README-template.md* to *README.md*

- Begin coding.

### Note

- The code in the */example* folder produces an app called Dem0App *Note the zero(0) in the name*

- The */example* app has:

1. A use case for ThemeManager for dark/light theme design
2. An example of dark/light switching via a button in the upper right corner
3. Localization using the package level */l10n .arb* files for localation key/values for shared use by both the package and *Dem0App*

- Localization can have errors after *flutter pub get* in how the l10n.yaml file is skipped because of ***bug*** during the flutter the build.

```dart
//*********************************************************************************
// If errors like 'Traget URI doesn't...' or 'Undefined name 'AppLocalizations'
// try 'flutter pub get' once more (or twice), or just run the app and they
// should disappear
//*********************************************************************************
```

## Useage

The 'example' directory is an app that includes:

- Usage of [flutter_block](https://pub.dev/packages/flutter_bloc)

- Usage of [flutter_modular](https://pub.dev/packages/flutter_modular)

- Localizations using [intl](https://pub.dev/packages/intl)

- User settable Light/Dark mode using [ThemeManager](https://github.com/GitHubStuff/theme_manager) {Tap the light-bulb in the upper right corner}

## Final note

Be kind to each other!
