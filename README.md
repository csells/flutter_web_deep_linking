# Flutter Web Deep Linking sample
This sample app shows off current best practices for handling deep linking, navigation and routing on the web when using Flutter. The same techniques also work in other Flutter apps, but they have fewer edge cases, e.g. you don't have to worry about people editing your route names in Flutter desktop because there's no address bar.

This code also has [a blog post](https://sellsbrothers.com/understanding-flutter-deep-links-on-the-web) that describes the principles used to produce it. I recommend starting there.

## Demo
You can try this sample app [here](https://csells.github.io/flutter_web_deep_linking/).

## Files
- **main.dart**: where the page widgets are defined, e.g. `PersonPage`
- **routers.dart**: where the `Router` helper is defined as well as the objects that know how to compose route names like `/family/452/person/42` and then to route them to the `PersonPage` with the appropriate famil and person object IDs
- **data.dart**: the simple data model that goes with this app

## Usage
To take advantage of this code, I recommend coping `routers.dart` into your project, tailoring it to fit your routable pages and then setting the `MaterialApp onGenerateRoute` property to `Router.onGenerateRoute`.

Enjoy.