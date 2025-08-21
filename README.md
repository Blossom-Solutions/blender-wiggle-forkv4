# Wiggle Bone (Blender 4.x Fork)

A minimal fork of the original Wiggle Bone add-on updated to work with Blender v4+.

---

## Changes in this fork
- Updated handler signatures to Blender 4 API:  
  `frame_change_pre/post`, `render_pre/post` now receive `scene`.
- Removed deprecated `IDPropertyGroup.to_dict()` usage; use the mapping directly.
- Fixed `FloatVectorProperty` defaults (tuples instead of `Vector(...)`) for 4.x type strictness.
- Simplified `frame_change_post` logic (no `depsgraph.view_layer` check).

---

## Install
1. Open **Blender** → **Edit** → **Preferences** → **Add-ons** → **Install…**  
2. Select `wiggle_bones.py` from this fork and enable it.

---

## Compatibility
- Tested with **Blender 4.x**.  
- Original behavior preserved; collisions remain labeled *experimental/disabled* in UI.

---

## Notes
- If any runtime error appears, share the error text and Blender version to iterate, or feel free to push an issue.  
