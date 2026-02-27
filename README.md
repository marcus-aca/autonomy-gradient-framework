# autonomy-gradient-framework

Public content and governance repository for the Autonomy Gradient language model and community blog submissions.

This repository is intentionally minimal and is used by `autonomy-gradient-app` as a blog content source.

## Source of Truth for App Blog Content

The app syncs from:

- `content/blogs`

At app build/test/dev time, blog markdown files in that directory are parsed and rendered in the app blog routes.

## Repository Structure

```text
autonomy-gradient-framework/
├── .github/
│   ├── CODEOWNERS
│   └── pull_request_template.md
├── model/
│   └── terms.yml
├── content/
│   └── blogs/
│       ├── README.md
│       ├── _template.md
│       └── *.md
├── CONTRIBUTING.md
├── LICENSE
├── LICENSE_SCOPE.md
└── README.md
```

## Governance

- Canonical terminology is maintained in `model/terms.yml`.
- Community blog submissions are accepted via PR into `content/blogs/`.
- Contributions are collaborative, with maintainers retaining final editorial and publication decisions.

See `CONTRIBUTING.md` for rights, editorial process, and submission requirements.

## License Model

Default license: CC BY-NC-ND 4.0.

Selected implementation-oriented files have explicit additional permissions to support practical adoption.

Exact scope and conditions are defined in:

- `LICENSE_SCOPE.md`

Commercial use rights and derivative rights for core framework content require explicit written approval from maintainers.
