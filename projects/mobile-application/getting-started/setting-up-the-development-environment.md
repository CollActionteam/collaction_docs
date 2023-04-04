# Setting up the Development Environment

If you are only interested in trying out the application, it is recommended you download the application from Appstore or Google Play. The documentation here will bring you through setting up a complete development environment.

## Cloning the project

First, you will have to clone the project. Open a terminal at your preferred location, or navigate to it.

Then clone the repository using this command:

```
git clone https://github.com/CollActionteam/collaction_app.git
```

If you are using SSH, you can clone the project using this command instead:

```
git clone git@github.com:CollActionteam/collaction_app.git
```

## Code generation

Due to the project using [freezed](https://pub.dev/packages/freezed), you will see a lot of errors when you open the project in your favorite editor. This is due to generated files not being tracked in git, thus needing to be generated. To do this see how to generate code in [Getting Started](https://docs.collaction.org/projects/mobile-application/getting-started#code-generation).

## Setting up Firebase Project

Refer to [Configuring Firebase](../../../configuring-firebase.md) for creating a Firebase Project.

_Remember to add the Google Service (JSON | PLIST) to the correct location as mentioned in Configuring Firebase._

## Environment secrets

To run the application, you must copy the `.env.example` and rename the copy to `.env`.&#x20;

_Remember to NOT REMOVE/RENAME the original file!_

The `.env` file is not tracked by Git, and will only exist on your local machine. If you are using a local version of the [Backend](../../backend/), you can use that for the `BASE_API_ENDPOINT_URL`. If not, you can find our development API on the [Public Environments](../../../public-environments.md) page.

The same goes for `BASE_STATIC_ENDPOINT_URL`, if you are hosting your own static bucket on AWS or Azure Blob, you can use that. Otherwise, you can the relevant development bucket on the [Public Environments](../../../public-environments.md) page.
