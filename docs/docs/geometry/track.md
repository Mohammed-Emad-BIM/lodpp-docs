# Track

Review how split layers differ from the archived source.

**Ribbon:** Geometry++ → Track  
**In Revit:** header **?** opens this page.

Track is a review tool. It does not rewrite geometry.

## What you see

Each row is a change since Split:

| Column | Meaning |
|--------|---------|
| Level | Level of the element |
| Role | Layer role |
| Change | What drifted |
| Archive | Design option or archive link label |

The window subtitle states the source: **Design option or Archive link only**.

## Workflow

1. Open **Track** after a Split that archived the originals.
2. Set the scope. If something is selected, the window starts on **Selection**. Otherwise it starts on **Active view**.
3. **Refresh** scans again. The window also scans when it opens.
4. Double-click a row, or press Enter, to zoom to that element.
5. **Level slice** puts a horizontal section box on the selected row's level.

An empty result means there is nothing to review in that scope.
