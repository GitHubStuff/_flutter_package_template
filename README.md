# empty_package

This is a template kit (with */example*) to create a Flutter Package.

The template project is a great foundation for creating packages that uses with BLoC and Modular programming patterns.

The package also contains an ad-hoc */example* folder with an app designed to load the new package and quickly allow the developer to create a demo/POC/beta-sample.

**^^The */example* that creates an app is also a great foundation for an app beyond development and proof-of-concept(POC)**

**Code Generation** Is key aspect of this package

---

## Setup

### Changes to content of template

- After un-ziping, rename the folder from _template_package to "new name"

- Rename 'lib/*empty_package.dart*' to the "new package name" (eg custom_widget_package.dart)

- Open the project in IDE of choice and search/replace "*empty_package*" with "new package name". This 100% works using VSCode.

- Search/Replace '*replace_domain*' with project/company domain.

#### NOTE

***replace_domain** will be part of the reverse domain used by XCode and Android in the app/product name. Choose carefully!*

- Localization: Search/Replace '*YYY*' with unique-ish three(3) uppercase characters. This will set a base of package-level localization that begin with YYY (eg YYYLocalization.HelloWorld)

- To create localization at the application level: Search/Replace '*XYX*' with unique-ish three(3) uppercase characters, that create localization like XYXLocalization.HelloWorld

***PAY ATTENTION 'YYY' vs 'XYX' => YYY: Package-level, XYX: Application-level***

- FINAL CRITICAL STEP

```text
 % !From the terminal run
 % flutter pub run build_runner build --delete-conflicting-outputs
```

This will build the ```lib/localizations/*.i69n.dart``` files, generate ```ib/localizations/dictionary_enum.g.dart```, ```lib/src/cubit/localization_cubit.g.dart``` at the package level.

At the **/example** level ```example/lib/cubit/localization_cubit.g.dart``` and ```example/lib/localization/dictionary_enum.g.dart```, and the ```example/lib/localization/*.i69n.dart``` files.

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
3. Localization using the package level ```/l10n``` are  ```.arb```  files for localation key/values for shared use by both the package and ```Dem0App```

### Language errors because Dart Analyzer crashed on VSCode

If errors like ```Traget URI doesn't...``` or ```Undefined name 'AppLocalizations'``` Reload the Dart Analyzer

1) Open the Command Palette (Ctrl+Shift+P)
2) Enter and select ```Developer: Reload Window```

## Useage

The 'example' directory is an app that includes:

- Usage of [flutter_block](https://pub.dev/packages/flutter_bloc)

- Usage of [flutter_modular](https://pub.dev/packages/flutter_modular)

- Localizations using [intl](https://pub.dev/packages/intl)

## Final note

Be kind to each other!
