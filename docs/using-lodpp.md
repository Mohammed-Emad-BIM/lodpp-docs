# Using LOD++

LOD++ commands follow one sequence: define the scope, review the list, then write. The footer states what the next action will change.

## Read, then write

| Action | Effect |
|--------|--------|
| Refresh, Scan, Customize | Reads the model. Nothing is written |
| Apply, Split, Divide, Replace, Delete, Pin, Unpin | Writes the checked rows |

Confirm the footer count before a write. Unchecked rows are left unchanged.

## Scope

Use the narrowest scope that still covers the work.

| Scope | When to use it |
|-------|----------------|
| Selection | The elements are already selected. Use this for the first run |
| Active view | The open view is the boundary |
| Whole model | Every matching element, including those not on screen |

## Undo

A completed write is a single Revit undo step. **Reset** restores the form. It does not reverse a write. Use Revit Undo for the model.

## Help and license

**?** opens the short guide for the open command, then the full page on this site. **About** shows the installed version and whether this seat is Free or Pro. Commands that require Pro say so on the button or in the footer.
