Create a COMPLETE, self-contained, single-file HTML document (everything inside one <html> block with embedded CSS and a massive <script> tag) that runs a fully interactive 3D WebGL scene titled "NEON VOID NAVIGATOR".

- Three.js, no external libraries. Include all matrix math utilities (mat4, vec3, etc.) inline as helper functions.
- Canvas fills the viewport. Retro CRT post-processing shader applied at the end: strong scanlines, chromatic aberration, vignette, barrel distortion, slight VHS jitter, and bloom approximation via multiple render passes.
- Scene: infinite scrolling magenta/cyan neon grid floor with perspective distortion. Procedural cyberpunk city blocks (extruded wireframe skyscrapers with glowing edge highlights). Dozens of floating holographic torii, icosahedrons, and rotating data cubes arranged in a Blade-Runner-meets-Matrix layout.
- Lighting: 8 animated point lights (hot pink, electric cyan, acid green, deep purple) that pulse, flicker, and move in sine-wave patterns. Full per-fragment Phong + rim lighting in the main shader with neon glow emission.
- Geometry complexity: procedurally generated buffers for grid (10,000+ vertices), buildings, and 50+ floating objects. Include simple particle system (GL_POINTS) for holographic data streams and glitch sparks.
- User inputs:
  • Mouse drag = orbit camera (spherical coordinates)
  • Mouse wheel = zoom
  • WASD = fly forward/strafe (first-person style movement)
  • Space = toggle "night-vision glitch mode" (intensifies scanlines + color inversion)
  • Left-click = spawn explosive neon particle burst at raycast position
  • Keyboard numbers 1–4 = switch between 4 different shader presets (classic neon, matrix rain overlay, wireframe only, full CRT)
- Animation: smooth 60 fps requestAnimationFrame loop with time-based pulsing, fog that reacts to light intensity, and subtle screen-space reflections on the grid.
- Retro HUD overlay (CSS + canvas text): flickering "NEURAL LINK: 98%" text, coordinates, "WARNING: SYSTEM OVERLOAD" that flashes on high movement, all in 80s synthwave font style (use system fonts that look cyberpunk).
- Full error handling, WebGL context creation with fallback, and a small on-screen instructions panel.

Output the complete HTML code in /home/neo/Documents/webGL-test/NEON_VOID_NAVIGATOR.html
