# Research API Documents

Content repository for the [HPD Research API Documentation](https://research-api-docs.hpdcollaborative.org) site. Each version branch contains the markdown documentation files and a `nav.json` file that defines the sidebar navigation for that version. No application code lives here.

The application that builds and serves this content is in the [research-api](https://github.com/HPDCollaborative/research-api) repository.

---

## Branch Structure

Each version of the API documentation is maintained as a separate branch. The default branch is always the current active version.

| Branch | Description                      |
| ------ | -------------------------------- |
| `3.0`  | Current active version (default) |
| `2.3`  | Previous version                 |
| `2.2`  | Legacy version                   |

> **Never merge version branches into each other.** Each branch is an independent snapshot of that version's documentation.

---

## Deployment

Pushing to any numbered version branch (e.g. `2.2`, `3.0`) automatically triggers a deployment via GitHub Actions. There is no need to touch any other branch.

New version branches are not publicly visible until a server administrator adds them to `DOC_VERSIONS` in the `.env` file on the production server. See [Publishing a New Version](#publishing-a-new-version) below.

---

## Directory Structure

Each version branch follows this structure:

```
├── index.md
├── nav.json
├── endpoints.md
├── faqs.md
├── repository-api.md
├── content/
│   ├── index.md
│   ├── locations.md
│   ├── materials/
│   ├── nested-materials/
│   ├── polymers/
│   └── substances/
└── data/
    ├── index.md
    ├── accessories.md
    ├── certifications.md
    ├── company.md
    ├── general.md
    ├── notes.md
    ├── parts.md
    ├── product/
    ├── reference.md
    └── voc.md
```

### Navigation

Nav titles in `nav.json` must be kept short or they will break the sidebar layout. If a title is too long, shorten it in `nav.json` and use the full title in the page's frontmatter instead.

### Frontmatter

Every `.md` file requires frontmatter:

```yaml
---
title: Page Title
category: Section Name
---
```

The root `index.md` of each version should also include the version number:

```yaml
---
title: Introduction
category: Introduction
version: '3.0'
---
```

---

## Updating Existing Documentation

1. Clone the repository:

   ```bash
   git clone git@github.com:HPDCollaborative/research-api-documents.git
   cd research-api-documents
   ```

2. Checkout the version branch you need to edit:

   ```bash
   git checkout 2.3
   ```

3. Make your changes, then commit and push:
   ```bash
   git add .
   git commit -m "Your change description"
   git push origin 2.3
   ```

Deployment triggers automatically on push.

---

## Publishing a New Version

1. Checkout the current latest version branch:

   ```bash
   git checkout 3.0
   ```

2. Create a new branch from it:

   ```bash
   git checkout -b 4.0
   ```

3. Update the `version` field in the root `index.md` frontmatter to reflect the new version.

4. Make your edits, then push:

   ```bash
   git push origin 4.0
   ```

5. Notify the Builder team. A server administrator must SSH into the production server and add the new version to `DOC_VERSIONS` in the `.env` file before it will appear on the live site. The administrator will also update the default branch on this repository to the new version.

---

## Important Rules

- **Never merge version branches into each other** — this will cause conflicts and break the documentation
- **Never delete the `.github/workflows` directory** from any branch — this is what triggers automatic deployments on push
- **Do not publish local builds** — all production deployments are handled automatically by the build server
