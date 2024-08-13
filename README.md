<div align="center">

# asdf-fastlane [![Build](https://github.com/mollyIV/asdf-fastlane/actions/workflows/build.yml/badge.svg)](https://github.com/mollyIV/asdf-fastlane/actions/workflows/build.yml) [![Lint](https://github.com/mollyIV/asdf-fastlane/actions/workflows/lint.yml/badge.svg)](https://github.com/mollyIV/asdf-fastlane/actions/workflows/lint.yml)

[fastlane](https://fastlane.tools) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`, `curl`, `tar`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).
- [Ruby](https://www.ruby-lang.org/en/) (>= 3.0)
- [Bundler](https://bundler.io): makes downloaded fastlane binary executable.

# Install

Plugin:

```shell
asdf plugin add fastlane
# or
asdf plugin add fastlane https://github.com/mollyIV/asdf-fastlane.git
```

fastlane:

```shell
# Show all installable versions
asdf list-all fastlane

# Install specific version
asdf install fastlane latest

# Set a version globally (on your ~/.tool-versions file)
asdf global fastlane latest

# Now fastlane commands are available
fastlane --help
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

### Important Notice

You must reinstall the fastlane plugin each time you change your Ruby version.

```shell
mise plugins uninstall fastlane -p
mise install
```

Do not install Ruby and the fastlane plugin simultaneously. The fastlane plugin requires certain gems to function properly, so the desired Ruby version should be set before installing the plugin.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/mollyIV/asdf-fastlane/graphs/contributors)!

# License

See [LICENSE](LICENSE)