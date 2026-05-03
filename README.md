# homeos-plugin-dnf

A [homeos](https://github.com/hainet50b/homeos) plugin for [DNF](https://github.com/rpm-software-management/dnf), the package manager used by Fedora, RHEL, and related distributions.

## Usage

Add the plugin to your homeos repository:

```sh
homeos plugin add dnf
```

Create a package using this plugin:

```sh
homeos package add neovim --plugin dnf --param name=neovim
```

## Parameters

| Parameter | Description |
|-----------|-------------|
| `name` | DNF package name (e.g., `neovim`) |

## Actions

| Action | Command |
|--------|---------|
| install | `sudo dnf -y install {{name}}` |
| update | `sudo dnf -y upgrade {{name}}` |
| uninstall | `sudo dnf -y remove {{name}}` |

## License

Licensed under either of

 * Apache License, Version 2.0
   ([LICENSE-APACHE](LICENSE-APACHE) or <http://www.apache.org/licenses/LICENSE-2.0>)
 * MIT license
   ([LICENSE-MIT](LICENSE-MIT) or <http://opensource.org/licenses/MIT>)

at your option.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
