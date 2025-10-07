# SOMA - Consciousness Meditation

A mystical, immersive meditation experience that combines breath work, 3D flower animations, and motion-responsive gradient filters. Experience consciousness through synchronized breathing, ambient sounds, and flowing visual effects.

## 🌟 Live Demo

[Experience SOMA →](https://somo-ar.vercel.app)

## 🧘‍♀️ Features

### **Square Breathing System**
- **4x4x4 breathing cycles** - Inhale (4s) → Hold (4s) → Exhale (4s) → Pause (4s)
- **Visual breathing guide** with pulsing energy rings
- **Countdown timer** for each phase
- **Synchronized flower animations** that grow and fade with your breath

### **Motion-Responsive Gradients**
- **Pink-to-blue gradient overlays** that follow your hand movement
- **Real-time motion detection** (no AI dependencies)
- **Breathing-synchronized intensity** - gradients pulse with your breath
- **TikTok-style filter effects** for immersive experience

### **Ambient Audio Experience**
- **Melodic pad sounds** with gentle harmonies
- **Breathing-synchronized tones** for each phase
- **Gentle chimes** and soft drones
- **Dynamic volume** that responds to breathing rhythm

### **Mystical UI Design**
- **Abstract, chic aesthetic** inspired by meditation apps
- **Glassmorphism effects** with soft glows
- **Dark gradient backgrounds** with flowing energy
- **Minimalist, shamanic** visual language

## 🚀 Quick Start

### **Local Development**
```bash
# Clone the repository
git clone https://github.com/candiikay/SomoAR.git
cd SomoAR

# Start local server
python3 -m http.server 8001

# Open in browser
open http://localhost:8001
```

### **Deploy to Vercel**
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

## 🎮 How to Use

1. **Begin Journey** - Click the start button
2. **Allow Camera Access** - For motion detection
3. **Follow Breathing Guide** - Watch the pulsing circle
4. **Wave Your Hands** - See gradients follow your movement
5. **Breathe Together** - Let the experience flow

## 🛠️ Technical Details

### **Built With**
- **Three.js** - 3D graphics and animations
- **Web Audio API** - Ambient sound generation
- **Canvas API** - Motion detection and gradient overlays
- **WebXR** - AR compatibility (with camera fallback)
- **Pure JavaScript** - No external AI/ML dependencies

### **Browser Support**
- ✅ **Chrome/Edge** - Full functionality
- ✅ **Firefox** - Full functionality  
- ✅ **Safari** - Camera and meditation features
- ✅ **Mobile** - Responsive design

### **Performance**
- **60fps animations** for smooth experience
- **Lightweight motion detection** - no heavy AI models
- **Optimized 3D models** for fast loading
- **Responsive design** for all screen sizes

## 🎨 Customization

### **Modify Breathing Patterns**
```javascript
// In garden.html, find startBreathingGuide()
const phases = [
  { name: 'Breathe In', duration: 4, action: 'inhale' },
  { name: 'Hold', duration: 4, action: 'hold' },
  { name: 'Breathe Out', duration: 4, action: 'exhale' },
  { name: 'Pause', duration: 4, action: 'pause' }
];
```

### **Change Gradient Colors**
```css
/* In garden.html, find .gradient-face-overlay */
background: linear-gradient(45deg, 
  rgba(255, 182, 193, 0.6),  /* Pink */
  rgba(173, 216, 230, 0.6),  /* Light blue */
  rgba(255, 182, 193, 0.6)   /* Pink */
);
```

### **Add Custom 3D Models**
```javascript
// Replace Flower.glb with your own GLTF model
const loader = new THREE.GLTFLoader();
loader.load('YourModel.glb', (gltf) => {
  // Your custom model setup
});
```

## 📱 Mobile Experience

SOMA is fully responsive and works great on mobile devices:

- **Touch-friendly** interface
- **Camera access** for motion detection
- **Optimized performance** for mobile browsers
- **Portrait/landscape** support

## 🔧 Troubleshooting

### **Camera Not Working**
- Ensure HTTPS connection (required for camera access)
- Check browser permissions
- Try refreshing the page

### **No Motion Detection**
- Check browser console for errors
- Ensure good lighting
- Try moving your hands closer to camera

### **Audio Not Playing**
- Check browser audio permissions
- Ensure device volume is up
- Try clicking on the page first

## 🌟 Philosophy

SOMA represents the intersection of technology and consciousness. It's designed to create a bridge between ancient breathing practices and modern digital experiences, helping users find moments of mindfulness in our connected world.

The name "SOMA" draws from ancient traditions - the divine drink of consciousness in Vedic culture, representing the essence of awareness and spiritual awakening.

## 📄 License

MIT License - feel free to use this project for your own meditation and wellness applications.

## 🤝 Contributing

Contributions welcome! Areas for improvement:
- Additional breathing patterns
- More gradient color schemes  
- Enhanced motion detection
- Mobile app version
- Social features

---

**Enter the void. Where breath becomes creation and consciousness blooms into existence.** 🌸✨
