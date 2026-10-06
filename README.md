# Unicross

Unicorns playing toss the ring with each other. A Unity 5.0 WebGL game from 2015.

Play it at https://unicross.jamey.xyz.

This is the built game only; the Unity project isn't here. Two fixes keep it running in current
browsers:

- `Release/unicross.js` was restored from the build's own gzipped copy after the served file was
  corrupted.
- `index.html` stubs out `setVelocity` on `AudioListener` and `PannerNode`, which browsers removed
  along with Web Audio's Doppler support.
