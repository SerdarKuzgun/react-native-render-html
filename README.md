<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>react-native-render-html</title>
    <style>
        body {
            text-align: center;
        }
    </style>
</head>
<body>

    <div>
        <a href="https://github.com/expo/expo">
            <img src="https://img.shields.io/badge/platforms-Android%20%7C%20iOS%20%7C%20MacOs%20%7C%20Windows-brightgreen.svg?colorB=191A17" alt="Platforms">
        </a>
        <a href="https://github.com/expo/expo">
            <img src="https://img.shields.io/badge/Runs%20with%20Expo-000.svg?style=flat&logo=EXPO&labelColor=ffffff&logoColor=000" alt="Runs with Expo">
        </a>
    </div>

    <div>
        <a href="https://www.npmjs.com/package/react-native-render-html">
            <img src="https://img.shields.io/npm/v/react-native-render-html/latest" alt="NPM Latest">
        </a>
        <a href="https://www.npmjs.com/package/react-native-render-html">
            <img src="https://img.shields.io/npm/v/react-native-render-html/next" alt="NPM Next">
        </a>
        <a href="https://www.npmjs.com/package/react-native-render-html">
            <img src="https://img.shields.io/npm/dm/react-native-render-html.svg?colorB=007ec6" alt="NPM Downloads">
        </a>
    </div>

    <div>
        <a href="https://codecov.io/gh/meliorence/react-native-render-html">
            <img src="https://img.shields.io/codecov/c/gh/meliorence/react-native-render-html" alt="Codecov">
        </a>
        <a href="https://github.com/meliorence/react-native-render-html/actions?query=branch%3Amaster+workflow%3ACI">
            <img src="https://github.com/meliorence/react-native-render-html/workflows/CI/badge.svg?branch=master" alt="CI Status">
        </a>
        <a href="https://github.com/meliorence/react-native-render-html/issues">
            <img src="https://img.shields.io/github/issues/meliorence/react-native-render-html.svg" alt="GitHub Issues">
        </a>
        <a href="https://semver.org/spec/v2.0.0.html">
            <img src="https://img.shields.io/badge/semver-2.0.0-e10079.svg" alt="SemVer">
        </a>
    </div>

    <div>
        <a href="https://discord.gg/dbEMMJM">
            <img src="https://img.shields.io/discord/736906960041148476?label=Discord" alt="Join Discord">
        </a>
        <a href="https://openbase.com/js/react-native-render-html">
            <img src="https://badges.openbase.com/js/rating/react-native-render-html.svg" alt="Rate on Openbase">
        </a>
    </div>

    <br>

    <a href="https://meliorence.github.io/react-native-render-html/">
        <img width="124" height="124" src="https://github.com/meliorence/react-native-render-html/raw/master/assets/logo.svg" alt="React Native Render HTML Logo">
    </a>

    <h1>react-native-render-html</h1>

    <p>
        <sup>Based on the original work of <a href="https://github.com/Thomas101">Thomas Beverley</a>, props to him.</sup>
    </p>

    <p>
        An iOS/Android pure JavaScript React Native component that renders your HTML into 100% native views.
    </p>

    <p>
        <a href="https://meliorence.github.io/react-native-render-html/blog/2021/06/27/create-blog-app-rnrh-I">
            <img width="320" height="744" src="https://github.com/meliorence/react-native-render-html/raw/master/assets/demo.gif" alt="Demo GIF">
        </a>
    </p>

</body>
</html>

### 🗃️ Releases

**The Foundry (v6) release is finally stable, and is now-on the recommended
version.** [Check out **the announcement blog post** in our brand new
website](https://meliorence.github.io/react-native-render-html/blog/2021/06/07/foundry-announcement).
We also have a [**migration
guide**](https://meliorence.github.io/react-native-render-html/docs/migration-guide)
for those who are coming from v5 and below.

> :warning: **You are on the master branch which is home for the latest development.**
> Check the table bellow to get documentation for your exact
> version.

| Minor | Branch                                                                                   | Documentation                                                                                              | Latest                                                                         |
| ----- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| next  | master                                                                                   | -                                                                                                          | [![npm](https://img.shields.io/npm/v/react-native-render-html/next)](#)        |
| 6.3   | [release/6.3](https://github.com/meliorence/react-native-render-html/tree/release/6.3)   | [Official Website](https://meliorence.github.io/react-native-render-html/)                                 | [![npm](https://img.shields.io/npm/v/react-native-render-html/release/6.3)](#) |
| 5.1   | [release/5.1](https://github.com/meliorence/react-native-render-html/tree/release/5.1)   | [release/5.1/README.md](https://github.com/meliorence/react-native-render-html/blob/release/5.1/README.md) | [![npm](https://img.shields.io/npm/v/react-native-render-html/release/5.1)](#) |
| 4.2   | [release/4.2](https://github.com/meliorence/react-native-render-html/tree/release/4.2)   | [release/4.2/README.md](https://github.com/meliorence/react-native-render-html/blob/release/4.2/README.md) | [![npm](https://img.shields.io/npm/v/react-native-render-html/release/4.2)](#) |

<a name="prereleases"></a>

## :computer: Install

```bash
npm install react-native-render-html
```

```bash
yarn add react-native-render-html
```

## :speedboat: Basic Usage

```jsx
import React from 'react';
import { useWindowDimensions } from 'react-native';
import RenderHtml from 'react-native-render-html';

const source = {
  html: `
<p style='text-align:center;'>
  Hello World!
</p>`
};

export default function App() {
  const { width } = useWindowDimensions();
  return (
    <RenderHtml
      contentWidth={width}
      source={source}
    />
  );
}
```

## :blue_book: Documentation

See our [official website](https://meliorence.github.io/react-native-render-html/) and [the official Discovery App](https://expo.io/@jsamr/react-native-render-html-discovery).

## :iphone: Example

You like to learn by example? We have a tutorial from which the demo GIF has been extracted: [A WebView-free Blog App with React Native Render HTML](https://meliorence.github.io/react-native-render-html/blog/2021/06/27/create-blog-app-rnrh-I).

## :notebook: Changelog

The changelog is available here: [packages/render-html/CHANGELOG.md](./packages/render-html/CHANGELOG.md).

## :bulb: Help

Please refer to [our dedicated document](./HELP.adoc).

## 👥 Community

You're always welcome to join our [discord channel](https://discord.gg/dbEMMJM) :-).

## :pencil: Contributing

Check-out our [contributing guide](./CONTRIBUTING.adoc).

- You can report bugs in [our Issue Tracker](https://github.com/meliorence/react-native-render-html/issues);
- We handle Feature Requests [in our Canny board](https://native-html.canny.io/features).

## :blue_heart: Sponsorship

Want to support this project or hire us to implement a feature? [Check out this page](https://github.com/sponsors/jsamr).

## :balance_scale: License

The source code is licensed under BSD 2-Clause "Simplified" License.
