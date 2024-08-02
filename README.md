# Drag

This is a fork from the crabnebula-dev/drag-rs, providing base support for drag
on OSX

- dropped GTK support altogether due to conflicting major deps
- moved the ns_window pointer as a function param rather than depending on the
  tauri v1 `window.raw_window_handle()` that can be used cross platform for OSX
  support
- dropped the `image: Image` param in favor of OSX default
- adjusted the API to be compatible with the V2 Tauri
- made `serde` dep required since it is used in one our Tauri app
