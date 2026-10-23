# killport Homebrew tap

Install the `killport-cli` alias to select this project's package without a
fully qualified formula name. The installed executable is still `killport`.

One-time setup and installation with Homebrew 6 or later:

```sh
brew tap paarths-collab/tap
brew trust --tap paarths-collab/tap
brew install killport-cli
killport --version
```

The trust command trusts this tap's current and future formulae and commands.
To trust only killport instead, replace that command with:

```sh
brew trust --formula paarths-collab/tap/killport
```

For subsequent upgrades:

```sh
brew update
brew upgrade killport-cli
```

The canonical `paarths-collab/tap/killport` formula and existing installations
remain supported. `killport-cli` is a relative symlink to that formula, so both
names use the same release, checksums and installation history. Preserve
`Aliases/killport-cli` when updating the generated formula.

Homebrew core's unqualified `killport` refers to another project. This alias
resolves package selection; both projects still install an executable named
`killport` and should not be linked into the same prefix simultaneously.

See Homebrew's [tap trust documentation](https://docs.brew.sh/Tap-Trust) and
[formula alias documentation](https://docs.brew.sh/Formula-Cookbook#a-quick-word-on-naming).

Packages v1.2.1 and later include the [MIT license](https://github.com/paarths-collab/killport/blob/v1.2.1/LICENSE). Historical releases retain their original license files.
