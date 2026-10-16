# 🍅 Tomato Leaf Doctor

An installable web app that classifies tomato leaf diseases from a photo. The model runs entirely in the browser (TensorFlow.js), so it works offline after the first load and no images are uploaded anywhere.

**Live demo:** https://YOUR-USERNAME.github.io/YOUR-REPO/
(On Android: open in Chrome, tap the ⋮ menu, then Install app / Add to Home screen.)

## About
- CNN trained in Python (TensorFlow/Keras) on 61,694 tomato leaf images across 11 classes
- 97.74% test accuracy on the held-out test split
- Model exported to TensorFlow.js format; front end in plain HTML, CSS and JavaScript
- Installable as a Progressive Web App (manifest + service worker), with camera and gallery input

## Limitations
- Trained on a public, curated dataset with clean images. Accuracy on real field photos (cluttered backgrounds, varied lighting) is likely to be lower.
- Educational demo, not a substitute for expert diagnosis.

## Project structure
- index.html: the app (UI + inference)
- model/: TensorFlow.js model files
- classes.json: class names in model output order
- manifest.json, sw.js, icon-*.png: PWA install and offline support

## Author
Sradhanjali Pradhan, M.Sc. Bioinformatics