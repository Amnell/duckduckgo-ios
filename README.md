# DuckDuckGo iOS

> [!IMPORTANT]  
> 👋 Thanks for your interest in DuckDuckGo! The source code for this project has been moved to [duckduckgo/apple-browsers](https://github.com/duckduckgo/apple-browsers) and this repo no longer accepts contributions.
> Please file any bug reports or feature requests in the new repo.

We are excited to engage the community in development!

## Building

### Submodules
We use submodules, so you will need to bring them into the project in order to build and run it:

Run `git submodule update --init --recursive`

### Developer details
If you're not part of the DuckDuckGo team, you should provide your Apple developer account id, app id, and group id prefix in an `ExternalDeveloper.xcconfig` file. To do that:

 1. Run `cp Configuration/DuckDuckGoDeveloper.xcconfig Configuration/ExternalDeveloper.xcconfig`
 2. Edit `Configuration/ExternalDeveloper.xcconfig` and change the values of all fields
 3. Clean and rebuild the project

### Dependencies
We use Swift Package Manager for dependency management, which shouldn't require any additional set up.

### SwiftLint
We use [SwifLint](https://github.com/realm/SwiftLint) for enforcing Swift style and conventions, so you'll need to [install it](https://github.com/realm/SwiftLint#installation).

## Debugging

### Instruments

We have a Custom Instruments tool to help visualize and track events that happen during runtime.

In order to run it:
1. Build a debug version and install it on a simulator or device.
2. Select the Instruments target and run it on a Mac. A new instance of the Instruments app will run. It will have a grayed out icon indicating that it works in debug mode with custom instruments attached.
3. Select the 'DDG Trace' template or set up a custom one by importing the 'DDG Timeline' instrument from Library.
4. Start recording.

See [Instruments Developer Help](https://help.apple.com/instruments/developer/mac/current/) for reference how to create custom instruments.

## Terminology

We have taken steps to update our terminology and remove words with problematic racial connotations, most notably the change to `main` branches, `allow lists`, and `blocklists`. Closed issues or PRs may contain deprecated terminology that should not be used going forward.

## Contribute

Please refer to [contributing](CONTRIBUTING.md).

## Discuss

Contact us at https://duckduckgo.com/feedback if you have feedback, questions or want to chat. You can also use the feedback form embedded within our Mobile App - to do so please navigate to Settings and select "Send Feedback".

## License
DuckDuckGo is distributed under the Apache 2.0 [license](https://github.com/duckduckgo/ios/blob/master/LICENSE.md).


