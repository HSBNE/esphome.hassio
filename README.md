# esphome.hassio
ESPHome config for site IOT / Smart Home automations.

# Layout
The directory structure of this repository is setup in a very specific way to
make for good reuses of commonly used devices and tooling used in deploying the
contained esphome configuration's.

**./modules**
Contains common yaml snippets that get reused over and over again in this
repository. The heavy lifting of configuring devices should be carried here with
per device files containing just enough to uniquely tune the specific device in
question.

**./**
The root of this repository should contain the per device yaml configurations
that draw as much as possible from common configuration base found in
`./modules`.
