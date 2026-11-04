# KV vertical services reel

Editable Hyperframes composition: `index.html`.
Output: `kv-reel.mp4` (1080×1920, 30 fps, 20 seconds, H.264 + AAC).

The reel uses the website's embedded fonts, service copy and SVG icons in a centered rounded browser frame on a red grid background. It is a services-focused motion adaptation, not a recording of the handling clip: the CloudFront source was inaccessible in the render environment. No vehicle footage is recreated.

The narration is in `voiceover.wav` (generated with the selected voice). Binary media is ignored by Git; retain it beside the composition when copying the project.

With Node.js 22+, Chrome and FFmpeg installed:

```sh
npx hyperframes@0.9.10 preview .
npx hyperframes@0.9.10 render . -o kv-reel.mp4 --fps 30 --quality delivery
```
