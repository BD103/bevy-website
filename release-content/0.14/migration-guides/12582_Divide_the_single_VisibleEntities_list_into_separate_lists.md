- `check_visibility` and `VisibleEntities` now store the four types of renderable entities–2D meshes, 3D meshes, lights, and UI elements–separately. If your custom rendering code examines `VisibleEntities`, it will now need to specify which type of entity it’s interested in using the `WithMesh2d`, `WithMesh`, `WithLight`, and `WithNode` types respectively. If your app introduces a new type of renderable entity, you’ll need to add an explicit call to `check_visibility` to the schedule to accommodate your new component or components.