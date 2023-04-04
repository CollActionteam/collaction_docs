# Getting Started

### Code Generation

In order to generate code related to `freezed`, `injectable`, `json_serializable`, etc. choose a command to run when you need to build or re-build these files:

_The watch command keeps re-building generated files. It is generally not recommended to use._

```
  flutter pub run build_runner watch --delete-conflicting-outputs
```

_If you want to build once you are done with your changes, to build generated files once run this command, it's preferred._

```
  flutter pub run build_runner build --delete-conflicting-outputs
```

### Immutable app settings

We use an environment file called `.env` to define secrets used in the application. These secrets are bundled with the application at build-time.

Make a copy of the `.env.example` file, name it `.env`, and fill out the missing secrets.
