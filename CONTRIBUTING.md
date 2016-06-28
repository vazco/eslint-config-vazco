# Making changes in the configs

## Modifying configs

Because making adjustments in this config could break tests/builds for several projects, all changes must be proceeded with caution.

To have high quality standards and keep developers happy at the same time, rules are democratically elected among Vazco team members.

To make a new change in the config:

- Create a Pull Request with links to ESLint documentation regarding new rules
- If you're a Vazco member: notify whole team at a daily meeting and via Slack
- Time for discussion and voting with thumbs up/down on the PR
- PR can be merged:
    - after 24h if > 50% `+1`
    - after 72h if `+1` > `-1`
    - there are no serious arguments against (discussion is over)
- PR can declined:
    - after 24h if < 50% `-1`
    - after 72h if `+1` < `-1`
- Update [CHANGELOG.md](CHANGELOG.md)
- Add new git tag (using `npm version`)
- Publish new version on NPM (check SemVer rules below)

## Adding new config sets

At the moment there is only one, `default` config.

New more specialized configs can added in the future by just adding new `.yaml` files.

E.g. create `example.yaml` (can be based on `default.yaml`) file in main directory and once published it could be imported in other projects:

```json
{
    "extends": "vazco/example"
}
```

## Versioning scheme

We use modified semver (_major_._minor_._patch_) scheme to better align with peer dependencies versions, especially with ESLint.

- Major​ version bump:
    - ESLint incompatible changes (eg. `eslint@2.x -> eslint@3.x`)
- Minor ​version bump:
    - New rule at `error` level
    - Anything else that could break previously passing tests
- Patch version bump​:
    - New rule at `warning` level
    - Removed rule
