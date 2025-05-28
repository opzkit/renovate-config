# renovate-config

Contains shareable config [presets](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
and [re-usable](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
Github workflow for [renovate](https://docs.github.com/en/actions/using-workflows/reusing-workflows).

The [default.json](./default.json) file contains the shared presets.

## Usage

Add a `.github/renovate.json` file with the following content:

```json
{
  "extends": ["github>opzkit/renovate-config"]
}
```

## Github/Organization setup
Renovate Github app [setup](https://docs.renovatebot.com/modules/platform/github/#running-as-a-github-app)
