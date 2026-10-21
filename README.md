# AirCanvas

Draw in the air using your webcam and index-finger tracking.

## Run it
Camera access requires HTTPS or localhost. The simplest test is to deploy this folder to a **private GitHub repository** and use a temporary GitHub Pages preview only if the repository/account settings allow it, or run locally with Python:

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Allow camera access.

## Features
- Browser-based hand tracking (MediaPipe Tasks Vision; CDN/model download required on first load)
- Pen, brush, marker, eraser
- Freehand, line, rectangle, ellipse
- Color picker, quick palette, brush size and opacity
- Undo, clear, live camera / white / black / transparent / custom-image background
- Export artwork as PNG
- Camera processing stays in the browser; no backend or account required

## Gestures
- Point with index finger extended and other fingers folded to draw.
- Lower the index finger / open your hand to pause the stroke.
- You can also use the mouse or touchscreen as a fallback while the camera is off.

## Notes
- Use good lighting and keep your hand in view.
- This is a first test build. Gesture accuracy and performance depend on webcam quality, browser, lighting, and hardware.
- Camera permissions require a secure context (HTTPS or localhost).
