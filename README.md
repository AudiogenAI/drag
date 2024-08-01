# Drag

This is a fork from the crabnebula-dev/drag-rs, aiming to support tauri v2 beta

- dropped GTK support altogether due to conflicting major deps
- moved the ns_window pointer as a function param rather than depending on the
  tauri v1 `window.raw_window_handle()` that can be used cross platform for OSX
  support
