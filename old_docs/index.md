

## Local data storage

All data it handles are saved to `hacs.*` files that is located under `.storage`

## HACS Sensor

During the setup HACS will add a new sensor to your installation (`sensor.hacs`).
This will have the number of pending updates as the state.

![sensor](https://user-images.githubusercontent.com/15093472/59136215-5ff29d00-8982-11e9-860f-75d382a4d3b7.png)

***

## Contribute

This integration is **massive** and there are a lot of areas to contribute to.

Contributions to the docs, will almost be blindly accepted.

_Contributions for the documentation should go against the `master` branch._

### For contributions to the integration itself (backend/frontend)

_Contributions for the integration should go against the `master` branch._

If the contribution is minor, make the change and open a PR (Pull Request).

For new features, changes to existing features, or other big changes, please open an RFC (Request for comment) issue before you start the work.

### Devcontainer

[The easiest way to contribute is to spin up a devcontainer.](https://code.visualstudio.com/docs/remote/containers) with VSCode, it has all the tools you need included, and it does not interfare with your system.

**Requirements:**

- Docker
- VS Code
- Remote - Containers (VS Code extention)

Make your changes, then run the task "Start Home Assistant" to test them, HA will run on port 8124.

***

## Last notes from the initial developer

First startup after installation will take some time, but it's worth it.

This was developed under the influence of 🍺, a lot of 🍺, [if you want to support my work feel free to buy me a ☕️ (most likely 🍺)](https://buymeacoffee.com/ludeeus)

How it works and what it does are added based on a single persons mindset, you may not agree with what I have done, if you have a suggestion please open an [RFC](https://github.com/custom-components/hacs/issues).

## Bugs / issues / suggestions

If you find bugs/issues or have any suggestions please open an issue in the [HACS Repository](https://github.com/custom-components/hacs/issues)