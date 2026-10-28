# The Smile That Fits

An interactive Lab 5 artwork about the pressure to appear happy to belong.

## Open the website

https://lishirley407-svg.github.io/smile-that-fits/

Click **Start camera**, allow camera access, then try smiling and relaxing your expression. No download or local server is needed.

## Run locally

1. Open this folder in VS Code.
2. Install the Live Server extension if needed.
3. Right-click `index.html` → **Open with Live Server**.
4. Use the localhost address, click **Start camera**, and allow camera access.
5. Smile, then relax your expression. The central creature blends into the crowd as the smile prediction rises; its orange color returns as the neutral prediction rises.
6. Click **Stop camera** when finished.

Internet access is required to load the libraries and hosted model. No build step is required.

## Model

https://teachablemachine.withgoogle.com/models/rYl40uxzD/

- Class 1: Smile
- Class 2: Neutral

The class selector lets you reverse the mapping if you retrain the model with a different class order. Keep both labels or update the selector when changing model labels.

Predictions describe resemblance to training examples; they do not measure happiness or identify people. The page processes camera frames in the browser and does not save or upload them. Background, lighting, and distance can influence predictions. Try untrained examples in similar lighting, then vary those conditions to assess generalization.

## Biomimicry and feedback

The work borrows camouflage, blending into surrounding colors, as an artistic analogy for social conformity. It does not equate the biological purpose of animal camouflage with human pressure to smile.

Expression → camera → trained image classifier → creature changes color → viewer observes → viewer changes or maintains expression.

## Deployment

GitHub Pages publishes the root directory of the `main` branch over HTTPS. The class assignment's separate Dokploy deployment remains pending; use a static application whose root contains `index.html`, and enable HTTPS for camera access.

## Libraries

TensorFlow.js 1.3.1 and Teachable Machine Image 0.8.3, following the official image-library example:
https://github.com/googlecreativelab/teachablemachine-community/tree/master/libraries/image
