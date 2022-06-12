# Repo Template

This repository is meant to serve as a general template for how to set up new repositories in the. In general, setting up a new repository should take only a few minutes; use this repository as a way of finding example files, and use the following checklist to ensure that you've set up the repository correctly.

## Install

These instructions are basic; you can use any method to do this work. The important part is making sure that you follow the checklist below before publishing the repository.

```sh
# Let's make a new folder
mkdir new-repo && cd new-repo
# Start a Git instance and copy over template files.
git init
cp ../repo-template/* .
```

## Checklist

Go through this checklist after creating your repository. It should only take a couple of minutes.

### README

- [ ] Update this `README.md` (Note, do last!).
- [ ] Rename all instances of `<Replace Title>` in README to match the new repo title
- [ ] Manually go through and edit the rest of the README.

### Other Files

- [ ] Copy `CODE_OF_CONDUCT.md` verbatim.
- [ ] Copy `CONTRIBUTING.md` and ensure that you've added any repository-specific instructions. (Replace `<Replace Title>` again).
- [ ] Should you have a `CHANGELOG.md`? Document your release process, if you plan on having one, in the `CONTRIBUTING.md` file.

### Dotfiles

- [ ] Do you need a `.gitignore` file?
- [ ] Do you need an `.npmignore` file?

### Licenses

- [ ] Copy the MIT license from the example repo.
- [ ] Have you added `MIT` as the license in the `package.json`?
- [ ] If you made changes, were these reflected in the last section of the README?

### GitHub Metadata

- [ ] Have you added a short description to the repository?
  - [ ] Is the description matched in the byline under the title in the README?
- [ ] Have you added topics to the GitHub repository?
  - [ ] Have you added these topics as keywords in the `package.json`?

### `package.json`

- [ ] Is the `author` field correct?
- [ ] Have you added `keywords`?
- [ ] Are the `bugs` and `homepage` fields correct?
- [ ] Have you added tests? Are they matched, here?
- [ ] Have you added a `lint` command?

### Tests

- [ ] Are there automated tests?
- [ ] ...for the browser as well?
- [ ] Are those reflected in CI?
- [ ] Bonus points: Using CircleCI workflows to segment tests?
- [ ] Extra bonus points: Are you cross-testing dependencies?

### Benchmarks

- [ ] Are there benchmarks?
- [ ] Did you run the benchmarks before / after the change or PR?

### Examples

- [ ] Is there an example folder with usage examples?
- [ ] For the browser as well?

## Contribute

If you think this could be better, please [open an issue](https://github.com/risadams/<Replace Title>/issues/new)!

Please note that all interactions in this organization fall under our [Code of Conduct](CODE_OF_CONDUCT.md).

## License

[MIT](LICENSE) © 1996+ Ris Adams
