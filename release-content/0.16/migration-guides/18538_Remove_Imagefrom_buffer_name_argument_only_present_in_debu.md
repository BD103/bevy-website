- `Image::from_buffer()` no longer has a `name` argument that’s only present in debug builds when the `"dds"` feature is enabled. If you happen to pass a name, remove it.
