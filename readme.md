# Multi-Timezone Flip Clock

A minimalist, animated flip clock for comparing times across multiple timezones. Perfect for scheduling international meetings and coordinating with teams around the world.

## Features

### ⏰ Core Functionality
- **Multiple Timezone Support** - Add and track unlimited timezones simultaneously
- **Animated Flip Display** - Smooth flip animations when time changes
- **24-Hour Format** - Clear military time display
- **Persistent Storage** - Your selected timezones are saved locally and restored on page reload

### 🎮 Time Controls
- **Hour Adjustment** - Jump forward/backward by 1 hour
- **Minute Adjustment** - Jump forward/backward by 10 minutes
- **Static Mode** - Time freezes when adjusted for easy meeting planning
- **Quick Reset** - Return to current time with one click

### 🎨 Design
- **Minimalist Interface** - Clean, distraction-free design
- **Dark Theme** - Easy on the eyes with orange accent colors
- **Mobile Responsive** - Works seamlessly on desktop, tablet, and mobile devices
- **Helvetica Typography** - Classic, readable font

### 🌍 Available Timezones
- **Americas**: New York, Chicago, Denver, Los Angeles
- **Europe**: London, Paris, Berlin
- **Middle East**: Dubai
- **Asia**: Mumbai/Delhi, Singapore, Tokyo, Shanghai, Hong Kong
- **Oceania**: Sydney, Auckland

## Demo

![Multi-Timezone Flip Clock Screenshot](https://edgarr.com/Multi-Timezone-Flip-Clock/)

## Usage

### Getting Started

1. **Open the file**
   - Simply open `multi-timezone-clock.html` in any modern web browser
   - No server or build process required!

2. **Add your first timezone**
   - Select a timezone from the dropdown menu
   - Click "Add Clock"
   - The clock will display the current time in that timezone

3. **Add more timezones**
   - Repeat the process to add as many timezones as you need
   - Each timezone can only be added once

### Time Adjustment

Use the control buttons at the bottom to adjust all clocks simultaneously:

- **+1h / -1h** - Adjust all clocks by 1 hour
- **+10m / -10m** - Adjust all clocks by 10 minutes
- **×** - Reset to current time and resume live updates

**Static Mode**: When you adjust the time, clocks enter "static mode" and display times rounded to the nearest 10 minutes (e.g., 14:30, 14:40). This makes it easy to visualize specific meeting times. Click the × button to return to live mode.

### Managing Clocks

- **Remove a clock** - Click the × button on the right side of any clock
- **View timezone** - Each clock displays the city name and timezone abbreviation (e.g., EST, JST)

## Technical Details

### Technologies Used
- **HTML5** - Structure
- **CSS3** - Styling and animations
- **Vanilla JavaScript** - Functionality (no frameworks required)
- **Intl API** - Timezone handling
- **localStorage** - Persistent data storage

### Browser Support
Works in all modern browsers that support:
- ES6 JavaScript
- CSS3 animations
- Intl.DateTimeFormat API
- localStorage

Tested on:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

### File Structure
```
multi-timezone-clock.html    # Main application file (all-in-one)
README.md                    # This file
```

## Responsive Design

The application is fully responsive with optimized layouts for:

- **Desktop** (>600px): Full-size flip cards with spacious layout
- **Mobile** (≤600px): Compact flip cards with optimized spacing and font sizes

## Customization

### Changing Colors
The orange accent color (#ff6b35) can be easily changed by finding and replacing all instances in the CSS.

### Adding More Timezones
Edit the timezone dropdown options and the `timezoneData` object in the JavaScript section:

```javascript
const timezoneData = {
    'America/New_York': 'New York',
    'Your/Timezone': 'Your City',
    // Add more here
};
```

## Future Enhancements

Potential features for future versions:
- Drag and drop to reorder clocks
- Custom timezone names
- Date display option
- 12-hour format toggle
- Export/import timezone configurations
- Share timezone links
- Dark/light theme toggle

## License

This project is open source and available under the MIT License.

## Credits

Inspired by classic flip clocks and modern timezone comparison tools like World Time Buddy.

---

**Built with ❤️ for remote teams and global collaboration**