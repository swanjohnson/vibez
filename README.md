# Daily Vibes - Your Personal Horoscope Reader

A simple, elegant, and mobile-friendly web application that delivers personalized daily horoscope readings using NFC tags or URL parameters. Discover your daily vibe, romantic compatibility, and celestial influences with a sleek, modern design.

## Features

- **Daily Horoscope Readings**: Unique messages generated daily for each zodiac sign, consistent throughout the day.
- **Best Romantic Match**: A new zodiac sign suggested daily for romantic compatibility.
- **Sun & Moon Signs**: Displays your sun sign and a daily rotating moon sign with elemental influences.
- **Color of the Day**: A fixed color associated with your zodiac sign.
- **Mood Prediction**: A characteristic mood for your sign.
- **Beautiful Design**: Gradient background, glassmorphism effects, and smooth animations.
- **Mobile-Friendly**: Optimized for smartphones, with PWA support for iOS.
- **NFC Tag Compatible**: Access your horoscope by scanning a zodiac-specific NFC tag.
- **Offline Functionality**: Runs entirely in the browser with no external dependencies.

## How to Use

1. **Via NFC Tag**: Scan your zodiac sign's NFC tag with a compatible device to load your horoscope.
2. **Via URL**: Visit the site directly with a URL parameter, e.g., `https://your-domain.com/?sign=leo`.
3. **Check Daily**: Return each day to see updated readings, romantic matches, and moon signs.

## Technical Details

- **Built With**: HTML, CSS, JavaScript
- **No Dependencies**: Fully self-contained, runs in the browser.
- **Daily Updates**: Uses a seeded random generator (`Math.sin`) based on the current date to ensure consistent yet daily-changing content.
- **Zodiac Data**: Static data for colors, moods, sun signs, and moon sign options; dynamic messages and matches generated daily.
- **URL Parameters**: Reads the `sign` parameter (e.g., `?sign=aries`) to determine the user's zodiac sign.
- **PWA Support**: Configured for standalone mode on iOS devices with full-screen display.

### How Daily Updates Work
- A `dateSeed` (YYYYMMDD format) drives the seeded random generator, ensuring:
  - Horoscope messages change daily but remain consistent within the day for each sign.
  - Romantic matches and moon signs update daily, staying consistent within the day.
- No external API calls are required, keeping it lightweight and offline-capable.

## Installation (For Developers)

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/daily-vibes.git