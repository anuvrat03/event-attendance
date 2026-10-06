# Instant Mobile Attendance System (Bongloor Venue)

A lightweight, high-speed, geo-fenced attendance tracking system designed for academic workshops and events. Built to prevent proxy attendance and maximize efficiency for participants using mobile devices.

## Features
- **Zero-Friction Entry:** Participants simply open a mobile web link, enter a 4-digit numeric code displayed on the presentation screen, and tap submit.
- **Strict Geo-Fencing:** Utilizes device GPS and the Haversine formula to enforce a strict 30-meter proximity perimeter around the venue (Bongloor, Telangana).
- **Automated Logging:** Instantly records verified attendance timestamps directly into a centralized Google Sheet via a Google Apps Script backend.
- **Mobile-Optimized:** Fully functional on mobile browsers, built and maintained entirely via mobile development tools (Samsung S20 FE, TrebEdit, GitHub Pages, and Google Workspace).

## Tech Stack
- **Frontend:** HTML5, CSS3, Vanilla JavaScript (Hosted on GitHub Pages).
- **Backend:** Google Apps Script Web App (`doPost` handler with CORS headers).
- **Database:** Google Sheets.

## Deployment & Usage SOP
1. **Presenter (Faculty):** Display the active 4-digit numeric code on the screen or projector.
2. **Participant:** 
   - Open the GitHub Pages link on their smartphone.
   - Ensure phone location/GPS permissions are enabled.
   - Enter the 4-digit code and tap **Submit Attendance**.
3. **Verification:** The system verifies proximity within 30 meters of the venue coordinates (`17.2352, 78.5831`) and automatically logs the entry into the Google Sheet.
