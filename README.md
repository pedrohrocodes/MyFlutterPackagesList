# My Flutter Packages List
Lista de packages principais/mais utilizo | Flutter

## Flutter Bloc | flutter_bloc
**Link:**
[flutter_bloc](https://pub.dev/packages/flutter_bloc)

## Google Fonts | google_fonts
**Link:**
[google_fonts](https://pub.dev/packages/google_fonts)

**Examples:**
```
Text(
  'This is Google Fonts',
  style: GoogleFonts.lato(),
), 
```
## Flutter SVG | flutter_svg
**Link:**
[flutter_svg](https://pub.dev/packages/google_fonts)

**Examples:**
```
SvgPicture.asset(
  assetName,
  color: Colors.red,
)
```

## Json Serializable | json_serializable
**Link:**
[json_serializable](https://pub.dev/packages/json_serializable)

**Examples:**
```
part of 'example.dart';

Person _$PersonFromJson(Map<String, dynamic> json) => Person(
      firstName: json['firstName'] as String,
      lastName: json['lastName'] as String,
      dateOfBirth: json['dateOfBirth'] == null
          ? null
          : DateTime.parse(json['dateOfBirth'] as String),
    );

Map<String, dynamic> _$PersonToJson(Person instance) => <String, dynamic>{
      'firstName': instance.firstName,
      'lastName': instance.lastName,
      'dateOfBirth': instance.dateOfBirth?.toIso8601String(),
    };
```

**Use:**
```
flutter pub run build_runner build
```

## Flutter Native Splash | flutter_native_splash
**Link:**
[flutter_native_splash](https://pub.dev/packages/flutter_native_splash)

**Examples:**
```
dev_dependencies:
  flutter_native_splash: ^1.2.4
```

```
flutter_native_splash:
 color: "#ffffff"
 image:
 android: true
 ios: true
```

**Use:**
```
flutter pub run flutter_native_splash:create
```

## Flutter Launcher Icons | flutter_launcher_icons
**Link:**
[flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)

**Examples:**
```
dev_dependencies:
  flutter_launcher_icons: ^0.9.2
```

```
flutter_icons:
  android: true
  ios: true
  image_path: 
```

**Use:**
```
flutter pub run flutter_launcher_icons:main
```

## Flutter Social Signin Buttons | flutter_signin_button
**Link:**
[flutter_signin_button](https://pub.dev/packages/flutter_signin_button)

**Examples:**
```
SignInButton(
  Buttons.Google,
  onPressed: () {},
)  
```

```
// with custom text  
SignInButton(
  Buttons.Google,
  text: "Sign up with Google",
  onPressed: () {},
)
```

```
SignInButton(
  Buttons.Facebook,
  mini: true,
  onPressed: () {},
)
```

<img src="https://github.com/ZaynJarvis/Flutter-Sign-in-Button/raw/master/showcase.png" height="600em"/>
