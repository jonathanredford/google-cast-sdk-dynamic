# google-cast-sdk-dynamic

ersion 4.6.1, the `google-cast-sdk` pod referenced the dynamically-linked version of the Google Cast iOS framework. This was a ~20MB download and a ~50MB framework.

Starting with 4.3.1, `google-cast-sdk` now refers to the statically-linked framework, which is a ~200MB download and a ~600MB framework, which makes for a poor developer experience.

This repo includes a podspec for the 4.6.1 dynamically-linked Google Cast iOS framework.

## Usage:

In your `Podfile`:

```ruby
pod 'google-cast-sdk-dynamic', :git => 'https://github.com/jonathanredford/google-cast-sdk-dynamic.git'
```

then `pod install`.
