# Merman Editor

## About
Merman is a mermaid diagram editor and also a file format. It extends conventional mermaid diagrams, which lack almost any information for layout (except some directionality of flow), with positional information that gives you some manual control over how a mermaid diagram is displayed. Begin by bringing a **mermaid** diagram into the workspace. You can do this by:

* Clicking the Open button to find a .mmd/.mermaid/.mmn/.merman file.
* Dragging a .mmd/.mermaid/.mmn/.merman file into the workspace.
* Pasting mermaid code into the syntax editor.

Saved **merman** files use a file format that appends layout details to the end of a standard mermaid file. You can always recover a mermaid file from a merman file by simply discarding the merman information after the obvious demarcation point in the file.

Currently, flowcharts (graphs) and classDiagrams are the best supported mermaid types. Other types might open correctly (sequenceDiagrams are confirmed) but might not be editable (or might not display correctly; I haven't tested them all yet).

## Commands
### Moving boxes and subgraphs
Drag any box or subgraph (a box containing boxes) to reposition it.

### Editing connections
Drag **connection endpoints** to reposition where connections attach to boxes.

**Option+drag** (Mac) or **Alt+drag** **connection endpoints** to reposition connections without snapping (in case they snap to an undesired location).

Drag **bezier control handles** to edit curves.

Drag **connection label handles** to reposition labels.

### Multi-object select
**Command+click** (Mac) or **Ctrl+click** to add/remove boxes and subgraphs to/from the selection for synchronized repositioning.

### Navigation
**Mouse-scroll** to zoom. **Space+drag** to pan. The **Fit** button nicely frames the diagram.

### Export
PNGs are exported in light mode. The **light/dark** button can assist with previewing, as can the **Show/Hide** controls button (the controls are still available when hidden and will appear when the cursor is nearby).

Support for exported SVGs is currently tenuous. Generated SVGs render to a varying degree of correctness by varying SVG tools.

### Contact
Merman was created by Keith Wiley (kwiley@keithwiley.com), mostly vibe-coded with Claude.

Repo: https://github.com/kebwi/merman_editor

Run it directly from Github without downloading or installing it: https://kebwi.github.io/merman_editor
