# PTZ Camera Controller
@ds1

## Overview

The PTZ Camera Controller is a web-based interface for controlling Pan-Tilt-Zoom (PTZ) cameras from your browser. It provides a responsive, intuitive user interface for precise camera movement control using mouse, keyboard, and touch inputs.

## Features

- **Multi-Device Camera Control**: Control PTZ cameras from any device with a modern web browser
- **Multiple Camera Sources**:
  - Placeholder image (for testing/demonstration)
  - Local webcam access (if available)
  - Network PTZ cameras
- **Intuitive Movement Controls**:
  - Pan (horizontal movement)
  - Tilt (vertical movement)
  - Zoom (in/out)
- **Multiple Input Methods**:
  - Mouse/trackpad drag gestures
  - Keyboard shortcuts
  - Touch gestures (mobile-friendly)
  - Direct value entry

## Control Methods

### Mouse Controls
- Left-click drag: Pan and tilt camera (or pan-only in axis lock mode)
- Right-click drag: Tilt-only (in axis lock mode)
- Scroll wheel: Zoom in/out

### Touch Controls
- Single finger drag: Pan and tilt (or pan-only in axis lock mode)
- Pinch gesture: Zoom in/out

### Keyboard Shortcuts
- **W**: Tilt up
- **S**: Tilt down
- **A**: Pan left
- **D**: Pan right
- **+/-**: Zoom in/out
- **R**: Reset camera position

### Direct Value Entry
Click on any value (Pan, Tilt, Zoom) to enter an exact value.

## Advanced Settings

### Inverted Tilt Mode
When enabled, inverts the tilt direction for mouse/touch control, providing more natural movement based on user preference.

### Axis Lock Mode
When enabled, restricts movement to one axis at a time:
- Left-click/drag for horizontal (pan) movement only
- Right-click/drag for vertical (tilt) movement only

## Technical Details

### Technologies Used
- Pure HTML, CSS, and JavaScript
- No external dependencies or libraries required
- Compatible with modern web browsers (Chrome, Firefox, Safari, Edge)
- Responsive design that works on desktop, tablet, and mobile devices

### Network Camera Support
- Secure credential storage (session-based)
- Automatic credential expiration for enhanced security

## Installation and Setup

1. Download the HTML file to your local machine or web server
2. Open the HTML file in a web browser
3. Select your preferred video source
4. For PTZ camera control:
   - Enter your camera's IP address
   - Provide authentication credentials
   - Start controlling your camera

## Security Considerations

- Camera credentials are stored in browser's sessionStorage (cleared when tab closes)
- Credentials have a 1-hour expiration time
- No data is sent to external servers other than your configured PTZ camera

## Future Enhancements

- Support for additional camera protocols
- Camera preset saving and recall
- Multi-camera management
- Recording capabilities
- Motion detection integration
