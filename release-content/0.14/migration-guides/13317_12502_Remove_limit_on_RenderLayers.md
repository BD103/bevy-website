There is no longer a limit on the total amount of `RenderLayers`, and so the `TOTAL_LAYERS` associated constant and `all()` constructor have been removed. Entities expecting to be visible on all layers, such as lights, should either create a constant listing all known layers used by the application or compute the active layers that are in use at runtime.

The `Copy` trait is no longer implemented on `RenderLayers`. Instead you should use the `.clone()` function from the `Clone` trait which `Renderlayers` still implements.
