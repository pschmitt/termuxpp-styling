# Termux:Styling

[![Build status](https://github.com/pschmitt/termuxpp-styling/workflows/Build/badge.svg)](https://github.com/pschmitt/termuxpp-styling/actions)
[![Join the chat at https://gitter.im/termux/termux](https://badges.gitter.im/termux/termux.svg)](https://gitter.im/termux/termux)

A TermuxPP add-on app to customize the terminal font and color theme. This fork
uses the Android package `dev.pschmitt.termux.styling` and must be signed with
the same certificate as TermuxPP core (`dev.pschmitt.termux`) to write the
required font or color files. Upstream/F-Droid builds target stock Termux and
are not interchangeable with this fork.

> **TermuxPP release channel:** New builds are published in the
> [TermuxPP monorepo](https://github.com/pschmitt/termuxpp/releases/tag/latest).
> Existing releases here remain available to older clients. See the
> [self-update guide](https://github.com/pschmitt/termuxpp/blob/main/docs/en/self-update.md).

When a style is selected, the app writes `font.ttf` or `colors.properties` to
`~/.config/termuxpp` if that directory exists, otherwise to the first existing
legacy directory, `~/.config/termux` or `~/.termux`. If none exists, it creates
`~/.config/termuxpp`. New configuration should use the canonical TermuxPP
directory.

## Installation

Termux:Styling application can be obtained from [F-Droid](https://f-droid.org/en/packages/com.termux.styling/).

Additionally we provide per-commit debug builds for those who want to try
out the latest features or test their pull request. This build can be obtained
from one of the workflow runs listed on [Github Actions](https://github.com/pschmitt/termuxpp-styling/actions/workflows/github_action_build.yml?query=branch%3Amaster+event%3Apush)
page.

Signature keys of all offered builds are different. Before you switch the
installation source, you will have to uninstall the Termux application and
all currently installed plugins. Check https://github.com/termux/termux-app#Installation for more info.

## How to use

1. When inside Termux, long press anywhere on the terminal.
2. Select `More...` in the resulting dialog.
3. Select `Style` in the next dialog.
4. Click either `CHOOSE COLOR` or `CHOOSE FONT` depending on what you want to customize.
