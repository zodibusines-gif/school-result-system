# School Result Management System - PWA

A comprehensive, offline-first Progressive Web App for managing student results, attendance, fees, and school administration.

## Features

### Core Modules
- 📊 **Dashboard** - Statistics, recent students, quick actions
- 👨‍🎓 **Student Management** - CRUD, profiles, filters by class/gender
- 👨‍🏫 **Staff Management** - Teacher/Principal/Admin roles with subject assignments
- 📚 **Class Management** - Nursery/Primary/Junior/Senior levels
- 📖 **Subject Management** - Subject codes and CRUD operations
- 📈 **Result Management** - Test 1 (20) + Test 2 (20) + Exam (60) = Total (100), auto-grading (A-F)
- 📋 **Report Cards** - A4 printable with school header, auto-generated comments
- 📊 **Broadsheet** - Class-wide results table with rankings
- ✅ **Attendance** - Daily marking, statistics dashboard
- 🎫 **ID Cards** - Gradient design, QR code, bulk print
- 🏆 **Certificates** - Graduation/Merit/Participation generator
- 📉 **Analytics** - Grade distribution, subject performance charts
- ⚙️ **Settings** - School config, session management, backup/restore

### Technology
- **Offline-First**: IndexedDB + Service Worker
- **PWA Ready**: Installable on mobile/desktop
- **Multi-Device Sync**: Share data with sync token
- **Session Restore**: Auto-return to last page
- **Form Recovery**: Unsaved forms restored
- **Responsive Design**: Mobile, tablet, desktop
- **PDF Export**: Reports, ID cards, certificates
- **Real-time Updates**: BroadcastChannel for same-device sync

## Installation & Usage

### Online Access
- Open: `https://school-result-system.netlify.app`
- Install as PWA (Add to Home Screen)

### Offline Usage
- App works completely offline after first load
- All data stored locally in IndexedDB
- Automatic sync when back online

### Multi-Device Access
1. Get a **Sync Token** from Settings
2. Share token with other users/devices
3. All changes sync automatically when online

## Roles & Access
- **Admin**: Full access, school settings, user management
- **Principal**: View reports, approve results, manage staff
- **Teacher**: Enter results, mark attendance, view analytics

## Login Credentials (Demo)
```
Admin:
- Email: admin@school.com
- Password: admin123

Teacher:
- Email: teacher@school.com
- Password: teacher123

Principal:
- Email: principal@school.com
- Password: principal123
```

## Folder Structure
```
school-result-system/
├── index.html           # Main PWA entry point
├── manifest.json        # PWA manifest
├── service-worker.js    # Offline service worker
├── css/
│   ├── style.css        # Main styles
│   └── print.css        # Print styles
├── js/
│   ├── app.js           # Main app logic
│   ├── db.js            # IndexedDB management
│   ├── auth.js          # Authentication
│   ├── sync.js          # Multi-device sync
│   ├── notifications.js # Alert system
│   └── modules/
│       ├── dashboard.js
│       ├── students.js
│       ├── staff.js
│       ├── classes.js
│       ├── subjects.js
│       ├── results.js
│       ├── reports.js
│       ├── broadsheet.js
│       ├── attendance.js
│       ├── idcards.js
│       ├── certificates.js
│       ├── analytics.js
│       └── settings.js
├── assets/
│   ├── logo.svg
│   └── icons/
└── docs/
    └── deployment.md
```

## Deployment

### Deploy to Netlify
1. Fork this repository
2. Connect to Netlify
3. Set build command: `npm install` (if needed)
4. Deploy!

Or drag & drop the folder to Netlify.

## License
MIT

## Support
For issues, feature requests, or questions, please open an issue on GitHub.
