# Pontoon-to-JSON
A build process CLI tool to convert the locale directory structure and .properties files output by [Pontoon](https://pontoon.mozilla.org) to JSON for use in JavaScript based l10n.

## Arguments

`--src` a directory to grab properties from. Defaults to `locales` at the project root

`--dest` a directory to output locales.json. Defaults to `dist` at the project root

## Config env

### 2.x
`SUPPORTED_LOCALES` a csv string with the locales to convert to json. Example `en-US, de, ja`. Defaults to `*`.

### 1.x
`SUPPORTED_LOCALES` an array with the locales to convert to json, or a string with a `*` for all. Example `["en-US", "de", "ja"]`. Defaults to `*`.
