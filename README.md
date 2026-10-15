# AI icons for NexLLM

Public SVG assets used by NexLLM through `custom:<id>` icon keys. The gateway needs the custom icon support update before these keys work.

## Add an icon

1. Upload a self-contained SVG to `icons/<id>.svg` on `main`.
2. Add `{ "id": "your-id", "label": "Display name" }` to the `icons` array in `icons.json`.
3. Refresh the NexLLM icon picker and select the name, or enter `custom:your-id`.

IDs must use lowercase ASCII letters, digits and hyphens, start with a letter or digit, and be at most 64 characters. Labels must be nonempty and at most 80 characters. The manifest supports up to 500 entries. Duplicate IDs are invalid.

Example: `icons/runware.svg` corresponds to `custom:runware`.

Icon content and manifest updates may take several minutes to appear because of GitHub/browser caching. No NexLLM image rebuild is needed for subsequent icon additions. Removing an entry from the manifest removes its suggestion; existing saved keys continue loading while the SVG remains available. Keep filenames stable to preserve saved keys.

SVGs are served as image resources, not inserted as inline markup. Use self-contained files without scripts, external fonts or external assets. Keep this repository free of credentials and private data. Existing LobeHub icon keys are independent of this repository.

## Sources

- `icons/runware.svg`: unchanged from [Runware/dify-runware, _assets/icon.svg](https://github.com/Runware/dify-runware/blob/main/_assets/icon.svg), Git blob `e8dcd3480e0c8ce67be1ef90edb704e3dd50deb1`, retrieved 2026-10-15. Runware branding belongs to its respective owner; no ownership of third-party logos is claimed.

- `icons/geodd.svg`: unchanged from [Geodd's official website logo](https://geodd.io/logo-geodd.svg), retrieved 2026-10-15. Use `custom:geodd`. Geodd branding belongs to its respective owner.
