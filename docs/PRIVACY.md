# Privacy Policy - DTU After Dark

**Last updated:** February 2026

## Data Collection

DTU After Dark does **not** transmit personal user data to third parties.

The extension operates locally in your browser. Some features store data locally to function (settings, caches, and user-entered data). If you enable Participant Intelligence, the extension may also store CampusNet participant list metadata (names, s-numbers, programs) and participant-count snapshots in `browser.storage.local` (you can toggle individual Participant Intelligence components on/off).

## What the Extension Does

- Injects CSS styles and JavaScript into DTU-related web pages to apply a dark color theme and additional features.
- All user preferences (dark mode toggle, bus configuration, GPA simulator data) are stored locally in your browser using localStorage and browser.storage.
- If Participant Intelligence is enabled, the extension reads participant lists on CampusNet pages you visit and stores derived data locally. Shared Course History and Semester Twins require storing participant metadata; Retention Radar stores enrollment-count snapshots. Optionally, Archive Backfill (on the CampusNet Group Archive page) can also fetch participant pages for archived courses to populate the same local dataset.
- No data leaves your device except as described under Third-Party Services below.

## Permissions

The extension requires access to the following domains to apply styling and features:

- `learn.inside.dtu.dk` - DTU Learn (Brightspace LMS)
- `s.brightspace.com` - Brightspace static assets (iframes)
- `sts.ait.dtu.dk` - DTU login page
- `evaluering.dtu.dk` - DTU course evaluations
- `studieplan.dtu.dk` - DTU study planner
- `kurser.dtu.dk` - DTU course catalog
- `karakterer.dtu.dk` - DTU grades
- `sites.dtu.dk` - DTU department sites
- `campusnet.dtu.dk` - CampusNet
- `sdb.dtu.dk` - Study line curriculum data (used for MyLine Curriculum Badges)
- `api.mazemap.com` - MazeMap room lookup (Smart Room Links)
- `www.bibliotek.dtu.dk` - DTU Library events and news

Some features read page content from these sites to provide functionality. Any stored data is stored locally in your browser. Personal data is not transmitted to third parties.

## Third-Party Services

The extension communicates with the **Rejseplanen API** (`www.rejseplanen.dk`) to fetch public transit departure times for DTU-area bus stops. These requests contain only stop IDs — no user-identifying information is sent.

If you enable **Smart Room Links (MazeMap)**, the extension may communicate with the **MazeMap search API** (`api.mazemap.com`) when you click a detected room link to resolve a text location (e.g. `308-016`) into a numeric POI destination ID. These requests contain only the building/room query and the DTU campus ID (89) â€” no user-identifying information is sent.

If you use **MyLine Curriculum Badges**, the extension may fetch `https://sdb.dtu.dk/myline` (DTU domain) using your existing DTU login session to determine which course codes belong to your study line plan. The parsed course-code mapping is cached locally in extension storage; it is not sent to third parties.

If you use the **Library** dropdown, the extension communicates with the **DTU Library website API** (`www.bibliotek.dtu.dk`) to fetch upcoming events and latest news. These requests contain no user-identifying information. Results are cached locally for 6 hours.

## Disclaimer

**DTU After Dark is an unofficial, community-built extension. It is not affiliated with, endorsed by, or supported by the Technical University of Denmark (DTU), Arcanic, D2L/Brightspace, Rejseplanen, MazeMap, or any other service provider.**

The information displayed by this extension -- including but not limited to exam dates, registration deadlines, grade statistics, GPA calculations, bus departure times, course evaluation summaries, and room locations -- is derived from publicly available sources and may be **inaccurate, incomplete, or outdated** at any time.

**You must always verify critical information (exam dates, registration deadlines, grades, course requirements) through official DTU channels.** Do not rely solely on this extension for time-sensitive academic decisions.

The developer(s) accept **no responsibility or liability** for:
- Missed exams, deadlines, or registration periods
- Incorrect grade calculations or GPA estimates
- Inaccurate bus departure times or missed transit
- Wrong or outdated course evaluation data
- Incorrect room locations or booking information
- Any academic, financial, or personal consequences arising from the use of this extension

This extension is provided **"as is"** without warranty of any kind, express or implied. Use it at your own risk.

## Contact

If you have questions about this privacy policy, please open an issue on the GitHub repository.
