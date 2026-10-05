# LOD++ documentation site (MkDocs)

User-facing manuals for the Revit add-in. Developer plans stay in `docs/plans/` at the repo root.

## Local preview

```powershell
cd docs-site
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
mkdocs serve
```

Open http://127.0.0.1:8000

## Publish

**From repo root:**

```powershell
powershell -ExecutionPolicy Bypass -File scripts\build-docs.ps1 -Serve    # local preview
powershell -ExecutionPolicy Bypass -File scripts\build-docs.ps1           # build site\ only
powershell -ExecutionPolicy Bypass -File scripts\build-docs.ps1 -Deploy   # gh-pages branch
```

The public site is **https://mohammed-emad-bim.github.io/lodpp-docs/** (repository `Mohammed-Emad-BIM/lodpp-docs`). The product repository stays private.

```powershell
powershell -ExecutionPolicy Bypass -File scripts\publish-docs.ps1
```

That copies `docs-site` only, pushes `main`, and updates GitHub Pages. `LodProductInfo.DocsBaseUrl` already points at that site.
