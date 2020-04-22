# Making changes in the configs

## Modifying configs

Because making adjustments in this config could break tests/builds for several projects, all changes must be proceeded with caution.

Before adding or changing rules, make sure that other configurations that extend the changes do not overwrite them in undesirable way.

To have high quality standards and keep developers happy at the same time, rules are democratically elected among Vazco team members.

To make a new change in the config:

1. Create a Pull Request with your changes and links to ESLint documentation regarding new rules, using the PR template.
1. If you're a Vazco member: notify whole team via Slack and at the weekly meeting. Also mention Vazco teams inside PR description.
1. Now it's time for discussion and voting with thumbs up/down on the PR.
    - PR can be merged:
        - after 2 workdays, if over 50% of Vazco developers gives a thumb up
        - after 5 workdays, if number of thumbs up is greater than thumbs down
        - there are no serious arguments against (discussion is over)
    - PR can declined:
        - after 2 workdays, if over 50% of Vazco developers gives a thumb down
        - after 5 workdays, if number of thumbs down is greater than thumbs up

## Releasing new version

This is usually done by project maintainer.

1. Update peer and dev dependencies.
1. Update [CHANGELOG.md](CHANGELOG.md) with new changes for this release.
1. Add new git tag using `npm version` (check SemVer rules below).
1. Publish new version on NPM.

## Adding new config sets

At the moment there are two config, `default` and `prettier`.

New more specialized configs can added in the future by just adding new `.yaml` files in to the `configs` directory.

E.g. create `example.yaml` (can be based on `default.yaml`) file and once published it could be imported in other projects:

```json
{
    "extends": "vazco/example"
}
```

## Versioning scheme

We use modified SemVer (_major_._minor_._patch_) scheme to better align with peer dependencies versions, especially with ESLint.

- Major​ version bump:
    - ESLint incompatible changes (eg. `eslint@2.x -> eslint@3.x`)
- Minor ​version bump:
    - New rule at `error` level
    - New peer dependency / removed peer dependency
    - Major dependency bump
    - Anything else that could break previously passing tests
- Patch version bump​:
    - New rule at `warning` level
    - Removed rule
    - Relaxing existing rule
    - Minor dependency bump
    - Other backward compatible changes
