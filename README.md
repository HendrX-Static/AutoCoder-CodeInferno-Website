# The Curse of Kuroyama Forest (黒山の呪い)

A horror-themed interactive web experience that tells the story of the cursed Kuroyama Forest through an immersive combination of text, visual effects, and audio elements.

## Deployed Link
```
https://cursed-kuroyama.netlify.app
```

## Features

- Interactive horror story with Japanese folklore elements
- Dynamic visual effects including:
  - RGB shift text distortion
  - Ghost appearances
  - Bloody handprint traces
  - Glitch effects
  - Noise overlay
  - Image jumpscares
- Smooth scrolling animation option
- Background music toggle
- Responsive design for all screen sizes
- Start screen with dramatic entrance
- Auto-scroll feature with "Cursed Scroll" option

## Technical Implementation

### Core Technologies
- HTML5
- CSS3 with advanced animations
- Vanilla JavaScript
- Custom fonts (Zen Antique, Noto Serif JP)

### Visual Effects
- CSS animations and transitions
- Dynamic DOM manipulation
- Viewport-based triggers
- SVG masks for handprint effects
- Randomized ghost appearances
- Text distortion effects

### Performance Optimizations
- Efficient event listeners
- Throttled animations
- Local storage for user preferences
- Optimized asset loading
- Viewport-based rendering

## Setup Instructions

1. Clone the repository
2. Replace placeholder images:
   - Update all `src="/api/placeholder/..."` references with actual image paths
   - Add your horror-themed images named 1.jpg through 7.jpg
   - Add your background GIF as bgg.gif
3. Add your background audio:
   - Place your audio file in the project directory
   - Update the audio source in the HTML to match your file name

## File Structure

```
kuroyama-curse/
├── index.html
├── images/
│   ├── 1.jpg
│   ├── 2.jpg
│   ├── 3.jpg
│   ├── 4.jpg
│   ├── 5.jpg
│   ├── 6.jpg
│   ├── 7.jpg
│   └── bgg.gif
└── audio/
    └── bg_audio.mp3
```

## Customization

### Modifying Colors
The site uses CSS variables for easy color customization:
```css
:root {
    --blood: #8B0000;
    --shadow: #1a0000;
    --text: #ffffff;
    --bg: #000000;
}
```

### Adding New Chapters
To add new chapters, follow this structure:
```html
<div class="chapter">
    <h2 class="rgb-shift">Chapter Title</h2>
    <p>Chapter content...</p>
</div>
<div class="jumpscare-container">
    <img src="image.jpg" alt="Description" class="jumpscare-image">
</div>
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

Note: Some visual effects may vary across browsers. Test thoroughly in your target browsers.

## Performance Notes

- The site uses multiple layered animations and effects which may impact performance on lower-end devices
- Consider reducing animation complexity for better performance on mobile devices
- Audio autoplay is blocked by most browsers until user interaction

## Known Issues

- Audio autoplay requires user interaction due to browser policies
- Some visual effects may cause slight performance issues on mobile devices
- Glitch effects may appear differently across browsers

## Contributing

Feel free to submit issues and enhancement requests.

## License

This project is released under the MIT License.

## Credits

- Fonts: Google Fonts (Zen Antique, Noto Serif JP)
- Story and concept: Original creation
- Implementation: Custom development

---

**Note**: This is a work of fiction. Any resemblance to actual persons, living or dead, or actual events is purely coincidental.
