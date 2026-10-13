# Contributing

Thank you for helping make reading accessible.

> [!IMPORTANT]
> Zacess is pre-release. Issues and pull requests on [zacesshq/zacess](https://github.com/zacesshq/zacess) open with the first release. Until then, ideas, questions and feedback are welcome in [Discussions](https://github.com/zacesshq/.github/discussions) or by email to [contact@zacess.com](mailto:contact@zacess.com).

## Once contributions open

All development will happen in [zacesshq/zacess](https://github.com/zacesshq/zacess). The read-only copies of each part (`core`, `quality`, `app`, `website`, `extension` and `workers`) are published from it, so pull requests opened there cannot be merged.

1. Every change starts from an issue that says what "done" means.
2. Work on a branch named after its type and topic, such as `feat/pdf-import` or `fix/ocr-confidence`.
3. Commit messages follow [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `docs:`, `test:`, `refactor:` and `chore:`.
4. Open a pull request that closes its issue. It is squash merged once checks pass and it is reviewed.

## Sign your commits off

Code contributions are accepted under the [Developer Certificate of Origin](https://developercertificate.org/). Add a `Signed-off-by` line to every commit to confirm you wrote the change or have the right to submit it under the project's licence:

```sh
git commit -s -m "fix: flag a misread minus sign"
```

## What every change is held to

- **Accessibility is a requirement, not a feature.** Every interface change meets WCAG 2.2 AA, works with a keyboard alone and is checked with a screen reader. See [ACCESSIBILITY.md](ACCESSIBILITY.md).
- **Accuracy over appearance.** A change to import or OCR runs the document quality suite. A drop in accuracy blocks the merge.
- **Local first.** A feature works on the device unless it genuinely cannot. Anything that sends data to a server says so before it runs.
- **The original is the source of truth.** Converted content never replaces the original, which always stays one step away.

The full guide, with local setup and the checks to run, will live in the `zacess` repository.
