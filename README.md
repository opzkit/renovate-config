# renovate-config

Contains shareable config [presets](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
and [re-usable](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
Github workflow for [renovate](https://docs.github.com/en/actions/using-workflows/reusing-workflows).

The [default.json](./default.json) file contains the shared presets and the
[renovate.yaml](.github/workflows/renovate.yaml) contains the workflow.

## Usage
In the repository to use the shared config create a `.git/workflows/renovate.yaml` with content
like the one in this [repo](.github/workflows/renovate_local.yaml).

Replace `uses: ./.github/workflows/renovate.yaml` with:
`uses: opzkit/renovate-config/.github/workflows/renovate.yaml@main`

Then add a `.github/renovate.json` file with the following content:

```json
{
  "extends": ["github>opzkit/renovate-config"]
}
```

## Github/Organization setup
Renovate Github app [setup](https://docs.renovatebot.com/modules/platform/github/#running-as-a-github-app)

Organization level Github action secrets:
* `RENOVATE_APP_ID`
* `RENOVATE_PRIVATE_KEY`
