# 📸 PhotoBooth App

A modern, web-based photobooth application that captures photos and arranges them in a beautiful 1x3 photo strip format with a 3-second countdown timer.

## ✨ Features

- **Camera Integration**: Access your device's camera for real-time photo capture
- **3-Second Countdown**: Visual countdown timer before each photo capture
- **1x3 Photo Strip**: Three photos arranged vertically in a single strip
- **Modern UI**: Beautiful, responsive design with smooth animations
- **Download Functionality**: Save your photo strip as a PNG file
- **Reset Option**: Clear all photos and start over
- **Mobile Responsive**: Works perfectly on both desktop and mobile devices

## 🚀 How to Use

1. **Open the App**: Open `index.html` in a modern web browser
2. **Start Camera**: Click the "Start Camera" button and grant camera permissions
3. **Position Yourself**: Get ready in front of the camera
4. **Take Photos**: Click "Take Photo" - you'll see a 3-second countdown
5. **Repeat**: Take all 3 photos to complete your strip
6. **Download**: Click "Download Strip" to save your photo strip

## 📱 Browser Requirements

- Modern browser with camera support (Chrome, Firefox, Safari, Edge)
- HTTPS connection required for camera access (or localhost for development)
- Camera permissions must be granted

## 🛠️ Technical Details

### File Structure
```
photobooth/
├── index.html          # Main HTML file
├── css/
│   └── style.css       # Styling and animations
├── js/
│   └── photobooth.js   # Core functionality
└── README.md           # This file
```

### Technologies Used
- **HTML5**: Structure and semantic markup
- **CSS3**: Modern styling with gradients, animations, and responsive design
- **JavaScript ES6+**: Camera API, Canvas manipulation, and photo processing
- **Web APIs**: MediaDevices API, Canvas API, File API

### Key Features Implementation
- **Camera Access**: Uses `navigator.mediaDevices.getUserMedia()`
- **Photo Capture**: Canvas-based image capture from video stream
- **Countdown Timer**: JavaScript interval-based countdown with visual feedback
- **Photo Strip Generation**: Canvas-based composition of multiple photos
- **Download**: Blob-based file download with custom filename

## 🎨 Design Features

- **Gradient Backgrounds**: Beautiful color gradients throughout the interface
- **Smooth Animations**: CSS transitions and keyframe animations
- **Responsive Layout**: Grid-based layout that adapts to screen size
- **Modern Typography**: Google Fonts (Poppins) for clean, readable text
- **Interactive Elements**: Hover effects and visual feedback on all buttons

## 🔧 Customization

### Changing Countdown Duration
Edit the `startPhotoCapture()` method in `js/photobooth.js`:
```javascript
let count = 3; // Change this number to adjust countdown duration
```

### Modifying Photo Strip Layout
Adjust the dimensions in the `downloadPhotoStrip()` method:
```javascript
const photoWidth = 400;  // Width of each photo
const photoHeight = 300; // Height of each photo
const spacing = 20;      // Space between photos
```

### Styling Changes
All visual styling can be modified in `css/style.css`. The app uses CSS custom properties and modern layout techniques for easy customization.

## 🚨 Troubleshooting

### Camera Not Working
- Ensure you're using HTTPS or localhost
- Check that camera permissions are granted
- Try refreshing the page and granting permissions again

### Photos Not Saving
- Check browser download settings
- Ensure pop-up blockers are disabled
- Verify sufficient storage space

### Layout Issues
- Clear browser cache
- Ensure JavaScript is enabled
- Check browser console for errors

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Feel free to submit issues, feature requests, or pull requests to improve the photobooth app!

---

**Enjoy capturing your memories! 📸✨** 