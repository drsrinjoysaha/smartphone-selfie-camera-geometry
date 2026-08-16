# Smartphone Selfie Camera Geometry: A Reproducible Capture Protocol

A technical reference for developers, photographers, and imaging practitioners who need repeatable smartphone portrait capture.

This document concerns image geometry, camera settings, illumination, and reproducibility. It is not a diagnostic tool, a measurement device, or advice about health, appearance, or treatment.

## Why close selfies can look different

A close smartphone selfie often uses a wide-angle camera. When a camera is close to a three-dimensional subject, nearer regions occupy a larger angle of view than regions farther away. In a face-sized subject, this can make central features appear proportionally larger and peripheral features appear farther away.

The principal cause is **camera-to-subject distance**, not focal length alone.

A longer-equivalent lens has a narrower field of view. It can support a more natural-looking portrait when the camera is moved farther back and the image is framed appropriately. Changing lenses while leaving the camera in exactly the same position changes framing, but does not change perspective.

## Scope

Use this protocol when the goal is to minimize avoidable variation between portrait captures over time.

It is designed to standardize:

- Camera position and subject distance
- Lens or camera selection
- Framing and orientation
- Illumination and white balance
- Focus and exposure behaviour
- File naming and metadata retention

It does not create a calibrated three-dimensional model, establish physical measurements, or support medical, legal, forensic, or identity-verification decisions.

## 1. Equipment

Recommended minimum setup:

- Smartphone with a rear camera
- Stable tripod or fixed mount
- Neutral, matte background
- One consistent light source
- Floor marker for the subject position
- Optional: remote shutter or capture timer

Prefer the rear camera over the front-facing camera when practical. Rear-camera modules commonly provide more consistent image quality and may provide a moderate-telephoto option.

## 2. Camera geometry

### 2.1 Distance is the primary control

Choose a camera-to-subject distance that can be repeated. For head-and-shoulders framing, begin at approximately 1.5–2.5 metres and adjust for the available lens and room size.

Record the distance and use a physical floor mark or fixed tripod placement for future sessions.

Do not compare a close arm's-length selfie directly with an image made from a fixed, more distant camera position. They represent different projection geometries.

### 2.2 Lens selection

Use a camera mode that provides approximately 50–85 mm full-frame-equivalent framing when available. On many phones, this may correspond to a 2× or 3× rear-camera option.

This is a framing recommendation, not a guarantee of geometric accuracy. Smartphone cameras differ in sensor size, crop behaviour, computational processing, and lens design.

Avoid digital zoom when an optical or native camera option is available.

### 2.3 Keep capture mode constant

For a repeatable series, retain the same:

- Phone and camera module
- Lens selection or zoom setting
- Camera orientation
- Camera-to-subject distance
- Output resolution
- Portrait, HDR, beauty, retouching, and filter settings

Disable beauty filters, face reshaping, skin smoothing, and similar computational alterations. If HDR or other processing cannot be disabled, use the same mode consistently and document it.

## 3. Focus, exposure, and colour

### 3.1 Focus

Focus on a stable high-contrast point near the plane of interest, such as the nearer eye in a portrait. Where the phone supports it, engage focus lock after framing.

### 3.2 Exposure

Automatic exposure can vary between captures as the background and ambient illumination change.

Where supported:

1. Set exposure after the lighting is in place.
2. Lock auto-exposure.
3. Do not change the exposure compensation setting between sessions.

If the device does not offer an exposure lock, document the camera application and use the same lighting, background, and time-of-day conditions.

### 3.3 White balance and lighting

Use one stable source of illumination. A neutral LED or soft light around 5000 K can be practical, but consistency is more important than a specific Kelvin value.

Avoid mixed lighting, such as daylight plus warm indoor lamps. Mixed sources produce colour shifts that automated white balance may correct differently from one image to the next.

Record:

- Light type and placement
- Approximate source-to-subject distance
- Colour-temperature setting, if available
- Whether daylight was present

## 4. Positioning protocol

### 4.1 Fixed reference points

Create two physical markers:

- A tripod marker for the camera
- A floor marker for the subject

Set the camera lens close to eye level for a neutral reference view. Keep the phone level; avoid a strong upward or downward tilt.

Enable the camera grid if available. Use it to keep horizon and head position consistent.

### 4.2 Standard views

With the camera fixed, move the subject rather than the camera.

Capture these views:

1. `front` — subject faces the camera; head upright; shoulders square.
2. `left-oblique-45` — subject turns approximately 45 degrees left.
3. `right-oblique-45` — subject turns approximately 45 degrees right.
4. `left-profile-90` — subject turns approximately 90 degrees left.
5. `right-profile-90` — subject turns approximately 90 degrees right.

For all views, keep the camera height, camera position, lens selection, and lighting unchanged.

## 5. Capture cadence

The appropriate interval depends on the project. For a visual documentation project, choose a fixed schedule that reduces inconsistent ad-hoc captures, such as weekly or monthly.

A regular interval does not turn photographs into objective biometric measurements. It simply improves comparability within a consistently captured image set.

## 6. Data and version control

Use a stable file naming convention:

```text
YYYY-MM-DD_project_camera_lens_distance_view_lighting_v01.jpg
