# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased](https://github.com/golang-templates/seed/compare/v0.16.1...HEAD)

## [0.16.1](https://github.com/golang-templates/seed/releases/tag/v0.16.1)

### Fixed

- Improve GH workflows and Makefile. ([#217](https://github.com/golang-templates/seed/pull/217))

## [0.16.0](https://github.com/golang-templates/seed/releases/tag/v0.16.0)

### Added

- Use [go-acc](https://github.com/ory/go-acc). ([#208](https://github.com/golang-templates/seed/pull/208))
- Add [misspell](https://github.com/client9/misspell). ([#211](https://github.com/golang-templates/seed/pull/211))
- Document docker vs Git Bash workaround. ([#212](https://github.com/golang-templates/seed/pull/212))

### Changed

- Update golangci-lint configuration. ([#196](https://github.com/golang-templates/seed/pull/196))
- Update Visual Studio code configuration. ([#197](https://github.com/golang-templates/seed/pull/197))
- Migrate to ghcr.io. ([#203](https://github.com/golang-templates/seed/pull/203))
- Use SemVer version as release name. ([#206](https://github.com/golang-templates/seed/pull/206))
- Manual changelog. ([#207](https://github.com/golang-templates/seed/pull/207))
- Update Makefile. ([#210](https://github.com/golang-templates/seed/pull/210))
- Bump dependencies.

### Removed

- Remove VS Code Remote Container support. ([#199](https://github.com/golang-templates/seed/pull/199))
- Remove info about GoDownloader as it is deprecated. ([#202](https://github.com/golang-templates/seed/pull/202))
- Remove testify. ([#209](https://github.com/golang-templates/seed/pull/209))

### Fixed

- Add `workflow_dispatch` to all workflows. ([#204](https://github.com/golang-templates/seed/pull/204))
- Fix docker image name. ([#205](https://github.com/golang-templates/seed/pull/205))
- Fix CodeQL GH workflow permissions. ([#216](https://github.com/golang-templates/seed/pull/216))

## [0.15.0](https://github.com/golang-templates/seed/releases/tag/v0.15.0)

### Added

- Add [CHANGELOG.md](CHANGELOG.md) based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). ([#131](https://github.com/golang-templates/seed/pull/131))
- Add [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) based on [Contributor Covenant](https://www.contributor-covenant.org/version/2/0/code_of_conduct/). ([#133](https://github.com/golang-templates/seed/pull/133))

### Changed

- Refine the triggers for the `build` GitHub workflow. ([#130](https://github.com/golang-templates/seed/pull/130))
  - Automatic trigger for the `main` branch.
  - Automatic trigger for pull requests targeting the `main` branch.
  - Manual trigger via [`workflow_dispatch`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#workflow_dispatch) ([blog post](https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/)).
- Lock the runners' version the in `build` and `release` GitHub workflows. ([#130](https://github.com/golang-templates/seed/pull/130))
- Configure `golint` linter with `min-confidence: 0.8` to avoid [false positive "should have a package comment"](https://github.com/golangci/golangci-lint/issues/1556). ([#132](https://github.com/golang-templates/seed/pull/132))
- Configure `gocyclo` linter with `min-complexity: 15` with is a recommended value by [Go Report Card](https://goreportcard.com/). ([#132](https://github.com/golang-templates/seed/pull/132))
- Update [GoReleaser](https://github.com/goreleaser/goreleaser) to [0.164.0](https://github.com/goreleaser/goreleaser/releases/tag/v0.164.0). ([#129](https://github.com/golang-templates/seed/pull/129))

## [0.14.0](https://github.com/golang-templates/seed/releases/tag/v0.14.0)

### Added

- Build and push a Docker container image. ([#127](https://github.com/golang-templates/seed/pull/127))

### Changed

- Move the `main` package to the root directory. ([#127](https://github.com/golang-templates/seed/pull/127))
  - It is suggested to use the `cmd` structure if the repository builds more than one application.
- Update [.golangci.yml](https://github.com/golang-templates/seed/blob/v0.14.0/.golangci.yml). ([#127](https://github.com/golang-templates/seed/pull/127))
- Update [GoReleaser](https://github.com/goreleaser/goreleaser) to [0.162.0](https://github.com/goreleaser/goreleaser/releases/tag/v0.162.0). ([#126](https://github.com/golang-templates/seed/pull/126))
- Update [golangci-lint](https://github.com/golangci/golangci-lint) to [1.39.0](https://github.com/golangci/golangci-lint/releases/tag/v1.39.0). ([#125](https://github.com/golang-templates/seed/pull/125))
