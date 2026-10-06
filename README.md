# Event Attendance Verification Portal

A lightweight, mobile-friendly web application designed for academic events, faculty workshops, and student gatherings. It eliminates proxy attendance and saves valuable time by combining a randomized verification CAPTCHA with strict device-level GPS geo-fencing (30-meter proximity radius).

## 🚀 Key Features
* **Geo-Fence Security:** Verifies that attendees are physically present within 30 meters of the event venue using device GPS coordinates.
* **Dynamic CAPTCHA:** Generates a unique 6-character alphanumeric code per session to prevent automated or remote bot submissions.
* **Mobile Optimized:** Built to run seamlessly on modern smartphones directly through mobile browsers.
* **Zero Cost Deployment:** Hosted easily and for free via GitHub Pages.

## 🛠️ Technology Stack
* **Frontend:** HTML5, CSS3, Vanilla JavaScript (Geolocation API & Haversine Formula).
* **Hosting:** GitHub Pages.
* **Development Environment:** Built and tested entirely on mobile devices using TrebEdit and GitHub.

## ⚙️ Configuration & Setup
1. **Clone or Download:** Fork this repository or download the `index.html` file.
2. **Update Venue Coordinates:** Open `index.html` and modify the latitude and longitude variables to match your specific event location:
   ```javascript
   const VENUE_LATITUDE = your_latitude_here; 
   const VENUE_LONGITUDE = your_longitude_here; 
   const ALLOWED_RADIUS_METERS = 30; // Adjust radius if needed
