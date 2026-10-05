# Split

Turn a compound wall, floor, roof, or ceiling into separate elements from its layers.

**Ribbon:** Geometry++ → Split

![Split, wall layers](../../assets/split.jpg)

## Layout

| Area | What it does |
|------|----------------|
| Scope | Whole model, active view, or current selection |
| Host | All, Walls, Floors, Roofs, or Ceilings |
| Type list | Check the types to split. Filter the names above the list |
| Output walls | **Every layer**, or **Exterior / Core / Interior** |
| Layer stack | Order, function, material, and thickness. Drag a layer while you edit |
| Footer | **Undo** the last Split. **Split** runs the checked types |

The header line above the stack summarizes the selected type: layer count, total thickness, host function, and whether openings copy onto the core wall.

## Workflow

1. Choose scope and host. **Walls** is the view in the screenshot.
2. Refresh if the type list is empty.
3. Check the types. **All**, **None**, and **Invert** act on that list.
4. Pick **Every layer** or **Exterior / Core / Interior**.
5. On the stack, set each layer's role (Structure, Finish, Insulation, and so on). **Host** marks the layer that keeps the original host behavior. **Set** writes the thickness shown on the right.
6. **Split**.

Review skipped types before you run. Openings and joins follow the note on the selected type. They are not a separate checkbox in this window.

Use Track afterwards when you need to see drift against the archived source.

## Recommended workflows

**One wall type, in the view you can see**

1. Set scope to **Active view** and host to **Walls**.
2. Check a single type.
3. Read the line above the stack: layer count, thickness, and whether openings copy onto the core wall.
4. Choose **Exterior / Core / Interior** when you want three walls, or **Every layer** when each material must be its own wall.
5. **Split**. Undo is on the footer if that type was the wrong choice.

**Reorder a finish before you split**

1. Select the type.
2. On the stack, move Finish, Insulation, and Structure until the exterior side and the interior side match the wall you build on site.
3. **Host** stays on the structural layer that should keep the original host behavior.
4. **Set** writes the thickness shown on that row.
5. Split that type only. Repeat per type rather than checking every wall type on the first pass.

Whole model plus every type is the widest run. Use it after one type in one view has produced the walls you expect.
