# Getting Started

### Code generation

In order to generate code related to `freezed`, `injectable`, and `json_serializable` choose a command to run when you need to build or re-build these files:

The watch command keeps re-building generated files. It is generally not recommended to use.

```
  flutter pub run build_runner watch -d
```

If you want to build generated files once run this command, it's preferred.

```
  flutter pub run build_runner build -d
```

_Note: The argument `-d` is shorthand for `--delete-conflicting-outputs` introduced in build\_runner 2.3.0._

### Immutable app settings

We use an environment file called `.env` to define secrets used in the application. These secrets are bundled with the application at build time.

Make a copy of the `.env.example` file, name it `.env`, and fill out the missing secrets.

If you are missing the secrets required for the application to run, reach out to a team member.

### Firebase configuration

In order to use features provided by Firebase, download the corresponding `google-services.json` and `GoogleService-Info.plist` from the Firebase console project, and add them to the project files.

Phone authentication has to be enabled in the Firebase console.

You can find or add phone numbers to use for testing in the Firebase Console by navigating to Authentication > Sign-in method > Sign-in providers > Phone > Phone numbers for testing

### Generating open-source Licenses

To generate the OpenSource licenses dart file via [flutter\_oss\_licenses](https://pub.dev/packages/flutter\_oss\_licenses), run the command `flutter pub run flutter_oss_licenses:generate.dart lib/presentation/licenses/oss_licenses.dart` from the project root.

> Note: Run `flutter format .` once [oss\_licenses.dart](https://github.com/CollActionteam/collaction\_app/blob/development/lib/presentation/licenses/oss\_licenses.dart) is created.

### Tests and test coverage

We use [codecov](https://codecov.io/gh/CollActionteam/collaction\_app) to make it visible in PRs what the test coverage is, and what changes to the coverage have been made.

If you are using [Visual Studio Code](https://code.visualstudio.com/) you can install these two extensions:

* [Flutter Coverage](https://marketplace.visualstudio.com/items?itemName=Flutterando.flutter-coverage)
* [Coverage Gutters](https://marketplace.visualstudio.com/items?itemName=ryanluker.vscode-coverage-gutters)

Now when you run `flutter test --coverage`, you will be able to see the test coverage in the TESTING tab, under "FLUTTER COVERAGE".

Additionally, if you don't want to run `flutter test --coverage` to generate the lcov test coverage files manually, which Coverage Gutters uses to show you line-for-line coverage in files, and Flutter Coverage uses to show you test coverage percentages, you can change your settings.

Open up settings and search for `Flutter Test Additional Args` and add `--coverage`. Now when you run tests from VSCode in the TESTING tab, it will run it with the `--coverage` argument, and the Flutter Coverage will update accordingly.

Using Coverage Gutters, remember to hit "Watch" on the blue status bar on VSCode.

### Git hooks setup

We have set up Git hooks to prevent extra whitespace and other possible mistakes before pushing the code to your branch. Run the below command in the project root directory to copy the pre-push hooks to your local `.git` directory.

```
cp ./hooks/* ./.git/hooks/
```
