# DTU Learn Dark Mode

A Firefox extension that applies a dark theme to DTU Learn and other DTU web services. No more bright white backgrounds during late-night study sessions.

## Supported Sites

- **DTU Learn** (learn.inside.dtu.dk) - Brightspace LMS
- **DTU Login** (sts.ait.dtu.dk)
- **Course Evaluations** (evaluering.dtu.dk)
- **Study Planner** (studieplan.dtu.dk)
- **Course Catalog** (kurser.dtu.dk)
- **Grades** (karakterer.dtu.dk)
- **Department Sites** (sites.dtu.dk)

## Features

- Two-tier dark theme: dark backgrounds (#1a1a1a) with lighter card/widget surfaces (#2d2d2d)
- Comfortable text color (#e0e0e0) that preserves custom-colored content
- Readable link color (#66b3ff)
- Shadow DOM and iframe support for full coverage of Brightspace components
- Runs at document start for instant dark mode with no white flash

## Installation

### Firefox Add-ons (Recommended)

Install directly from the Firefox Add-ons store: *(link to be added after publishing)*

### Manual Installation (For Testing)

1. Open Firefox and navigate to `about:debugging`
2. Click "This Firefox" in the left sidebar
3. Click "Load Temporary Add-on..."
4. Select the `manifest.json` file from this folder
5. Visit [learn.inside.dtu.dk](https://learn.inside.dtu.dk) to see the dark mode

**Note:** Temporary add-ons are removed when you close Firefox.

## Files

- `manifest.json` - Extension manifest (Manifest V2)
- `darkmode.css` - CSS dark mode styles (loaded at document start)
- `darkmode.js` - JavaScript for dynamic element styling, shadow DOM injection, and iframe handling
- `logo_dark.png` - Extension icon
- `PRIVACY.md` - Privacy policy
- `LICENSE` - MIT License

## Customization

Edit `darkmode.css` to tweak the color scheme:

| Element         | Color     |
|-----------------|-----------|
| Main background | `#1a1a1a` |
| Cards/widgets   | `#2d2d2d` |
| Text            | `#e0e0e0` |
| Links           | `#66b3ff` |

After making changes, reload the extension in `about:debugging`.

## Privacy

This extension does not collect, store, or transmit any user data. All processing happens locally in your browser. See [PRIVACY.md](PRIVACY.md) for full details.

## License

MIT License. See [LICENSE](LICENSE).

## Contributing

Found an element that still has a bright background? Open an issue or submit a pull request.

---

Made for DTU students who study after dark.
