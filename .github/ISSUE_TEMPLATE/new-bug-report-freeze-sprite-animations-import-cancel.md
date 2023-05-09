---
name: .github/ISSUE_TEMPLATE
about: Use this option to report a bug. You must use this option for your report to
  be investigated.
title: 'Freeze on sprite animations import cancel'
labels: ''
assignees: ''

---

<!-- You must use this template or your issue will be closed without investigation. Please see the guidelines. -->

## Problem description

In 336 stable, when editing a sprite's animation frames, if you right-click > import frames > from files or from strip, then cancel the explorer window, and then close the animations editor, Construct will freeze.

## Attach a .c3p

<!-- A minimal Construct project (.c3p) is required to be attached. Your issue will likely be closed without investigation if you don't provide one. Please see the guidelines -->
https://drive.google.com/file/d/1i0o85TQLYKQ53gnaxBrz3l-K_saJeZW2/view?usp=share_link 

This issue happens in a literal complete new file

## Steps to reproduce

1. Double click the example sprite in the project, or right-click, New Object, Sprite, and Add and click to add it to the layout
2. In the sprite animations editor window, right click in the "animation 1 frames" mini-window, then choose Import Frames..., then choose "From Files" or "From Strip"
3. Navigate your explorer window anywhere (or nowhere, doesn't matter), then press Cancel
4. Close the animations editor window.

## Observed result

Construct immediately "soft freezes" -- You can change the size of the animations editor window, but your mouse will be stuck in a loading cursor and the window will not close. The screen dims slightly as it does when you close the animation window, but it never lightens back up because the window never closes. You cannot navigate anywhere else in the project. You cannot save the project. The only option is to close and re-open the project.


## Expected result

The expected result is that the animations editor window will close without any changes happening to the sprite.

## More details

This issue happens in Chrome, Firefox, and Opera in Windows at least (those are the three that I've tried it on). 


**Affected browsers/platforms:** <!-- Chrome/Firefox/Safari, Windows/macOS/Android, etc -->

Windows 10 Chrome
Windows 10 Firefox
Windows 10 Opera

**First affected release:** <!-- e.g. worked in r122 but broke in r123 -->
I'm afraid I don't know the first affected release. I only started experiencing it in the last week, though I don't know if that was because it's a recent bug or if it's because I've never cancelled an import before. 
## System details

<!-- If you see a crash report dialog, please copy and paste it to where it says "PASTE HERE" below. -->
<!-- Otherwise please go to Menu > About > Platform information and paste that information there instead. -->

<details><summary>View details</summary>

Platform information
Product: Construct 3 r336 (stable)
Browser: Chrome 111.0.5563.148
Browser engine: Chromium
Context: browser
Operating system: Windows 10
Device type: desktop
Device pixel ratio: 1
Logical CPU cores: 12
Approx. device memory: 8 GB
User agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36
Language setting: en-US

Local storage
Storage quota (approx): 142 gb
Storage usage (approx): 101 mb (0.1%)
Persistant storage: No

Browser support notes
This list contains missing features that are not required, but could improve performance or user experience if supported.

Nothing is missing. Everything is OK!
WebGL information
Version string: WebGL 2.0 (OpenGL ES 3.0 Chromium)
Numeric version: 2
Supports NPOT textures: yes
Supports GPU profiling: yes
Supports highp precision: yes
Vendor: Google Inc. (AMD)
Renderer: ANGLE (AMD, AMD Radeon RX 5700 XT Direct3D11 vs_5_0 ps_5_0, D3D11)
Major performance caveat: no
Maximum texture size: 16384
Point size range: 1 to 1024
Extensions:

EXT_color_buffer_float
EXT_color_buffer_half_float
EXT_disjoint_timer_query_webgl2
EXT_float_blend
EXT_texture_compression_bptc
EXT_texture_compression_rgtc
EXT_texture_filter_anisotropic
EXT_texture_norm16
KHR_parallel_shader_compile
OES_draw_buffers_indexed
OES_texture_float_linear
OVR_multiview2
WEBGL_compressed_texture_s3tc
WEBGL_compressed_texture_s3tc_srgb
WEBGL_debug_renderer_info
WEBGL_debug_shaders
WEBGL_lose_context
WEBGL_multi_draw
Audio information
System sample rate: 48000 Hz
Output channels: 2
Output interpretation: speakers
Supported decode formats:

WebM Opus (audio/webm; codecs=opus)
Ogg Opus (audio/ogg; codecs=opus)
WebM Vorbis (audio/webm; codecs=vorbis)
Ogg Vorbis (audio/ogg; codecs=vorbis)
MPEG-4 AAC (audio/mp4; codecs=mp4a.40.5)
MP3 (audio/mpeg)
FLAC (audio/flac)
PCM WAV (audio/wav; codecs=1)
Supported encode formats:

WebM Opus (audio/webm; codecs=opus)
Video information
Supported decode formats:

WebM AV1 (video/webm; codecs=av01.0.00M.08)
MP4 AV1 (video/mp4; codecs=av01.0.00M.08)
WebM VP9 (video/webm; codecs=vp9)
WebM VP8 (video/webm; codecs=vp8)
Ogg Theora (video/ogg; codecs=theora)
H.265 (video/mp4; codecs=hev1.1.2.L93.B0)
H.264 (video/mp4; codecs=avc1.42E01E)
Supported encode formats:

WebM VP9 (video/webm; codecs=vp9)
WebM VP8 (video/webm; codecs=vp8)

</details>
