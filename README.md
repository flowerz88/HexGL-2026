HexGL 2026
=========

This is new 2026 version of the original [HexGL](http://hexgl.bkcore.com), the futuristic HTML5 racing game by [Thibaut Despoulain](http://bkcore.com)

Demo (note: translated in Dutch) is available [here]|https://www.komchatten.nl/games/zweefracer].

## Major changes
Modernized mobile support and caching for HexGL.

Changes include:
- Replaced the old mobile button controls with a full screen gesture based touch layer.
- Touch controls now use hold to accelerate, drag left/right to steer and swipe down to brake/drift.
- Added modern touch detection using navigator.maxTouchPoints and coarse pointer checks.
- Added optional orientation control support with permission handling for modern mobile browsers.
- Improved mobile defaults by selecting touch controls and low quality on touch devices.
- Added mobile audio unlock/resume handling after user interaction.
- Added cache busting query versions for changed JS/CSS files.
- Removed reliance on deprecated AppCache / Firefox OS packaging files.
- Added safer .htaccess caching rules for static game assets while keeping HTML revalidated.

The goal is to make the original HexGL code more usable on modern mobile browsers without rewriting the rendering engine or upgrading the legacy Three.js stack.

## License

Unless specified in the file, HexGL's code and resources are now licensed under the *MIT License*.

## Installation

	cd ~/
	git clone git://github.com/BKcore/HexGL.git
	cd HexGL
	python -m SimpleHTTPServer
	chromium index.html

To use full size textures, swap the two textures/ and textures.full/ directories.
