# SKO26 Seating Chart - Complete Directory

## 📋 Overview

Professional, Appian-branded alphabetical seating directory for the **SKO26 (Sales Kickoff 2026)** event. Features real-time search, responsive design, and complete information for all 128 attendees across 18 tables.

---

## 🎯 Event Information

- **Total Attendees:** 128
- **Total Tables:** 18 (7-8 seats each)
- **Theater Regions:** CNA, EMEA, USPS, APJ, SPEAR
- **Format:** Alphabetical directory with search
- **File:** Single HTML file (no dependencies)

### Theater Distribution
- **CNA:** 47 attendees (including Campell-Balcombe, Paul)
- **EMEA:** 33 attendees
- **USPS:** 27 attendees
- **APJ:** 13 attendees
- **SPEAR:** 8 attendees

---

## 🚀 Quick Start Guide

### Option 1: Open Locally (Easiest)
1. Download the `index.html` file
2. Double-click to open in your web browser
3. Start searching! No setup required

### Option 2: Deploy to Web (For Event Attendees)
Choose any free hosting platform:

#### **GitHub Pages** (Recommended for teams)
```bash
1. Create a new repository on GitHub
2. Upload index.html
3. Go to Settings → Pages
4. Select "main" branch → Save
5. Your URL: https://[username].github.io/[repo-name]
```

#### **Netlify** (Fastest deployment)
```bash
1. Visit netlify.com
2. Drag and drop index.html
3. Get instant public URL
4. Share with attendees
```

#### **Vercel** (Enterprise-grade)
```bash
1. Visit vercel.com
2. Upload index.html
3. Get instant public URL with SSL
4. Professional domain available
```

#### **Company Web Server**
```bash
1. Upload to your Appian web server
2. Place in public or intranet directory
3. Share internal URL with attendees
4. Optionally restrict to VPN/internal access
```

---

## ✨ Features

### Core Features
- ✅ **128 Attendees** - Complete, up-to-date list
- ✅ **Real-time Search** - Find anyone instantly
- ✅ **Alphabetical Sorting** - Easy to browse
- ✅ **Table Assignments** - Clear table numbers (1-18)
- ✅ **Theater Information** - CNA, EMEA, USPS, APJ, SPEAR
- ✅ **Job Titles** - Role information for networking

### Design Features
- 🎨 **Appian Branding** - Official colors (#00A6E0, #212B35)
- 📱 **Mobile-Friendly** - Responsive on all devices
- 🖨️ **Print-Optimized** - Clean printouts
- ⚡ **Fast Loading** - <1 second load time
- 🔒 **Offline-Ready** - Works without internet (after initial load)
- ♿ **Accessible** - Semantic HTML, keyboard navigation

---

## 🔍 Using the Search Feature

The search box provides instant filtering across all attendee information.

### Search Examples

**Find by Name:**
```
Type: "smith"
Results: All attendees with "Smith" in their name
```

**Find by Theater:**
```
Type: "EMEA"
Results: All 33 EMEA attendees
```

**Find by Title:**
```
Type: "director"
Results: All Directors across all theaters
```

**Find by Table:**
```
Type: "5"
Results: All attendees assigned to Table 5
```

### Search Tips
- 🔤 Case doesn't matter (smith = Smith = SMITH)
- ⚡ Results update as you type
- 🎯 Searches across all fields simultaneously
- 🗑️ Clear search box to see all attendees again

---

## ✏️ Updating Attendee Information

### Adding a New Attendee

1. Open `index.html` in any text editor (Notepad, VS Code, Sublime, etc.)
2. Find the `attendees` array (approximately line 255)
3. Add new entry in alphabetical order by last name:

```javascript
{name: "Doe, Jane", table: 10, theater: "CNA", title: "Senior SC"},
```

4. Update the total count (line 256):
```html
<div class="stat-number">129</div>
```

5. Save file and refresh browser

### Updating Existing Attendee

1. Open `index.html` in text editor
2. Find the attendee in the `attendees` array
3. Modify their information:

```javascript
// Before
{name: "Smith, John", table: 5, theater: "CNA", title: "SC"},

// After
{name: "Smith, John", table: 8, theater: "EMEA", title: "Senior SC"},
```

4. Save and refresh

### Removing an Attendee

1. Find their entry in the `attendees` array
2. Delete the entire line (including comma)
3. Update total count to reflect new number
4. Save and refresh

---

## 🎨 Customization Guide

### Change Appian Brand Colors

Locate the CSS section (around line 20) and modify:

```css
/* Primary Blue - Headers, buttons, highlights */
.header { background: #00A6E0; }
.table-number { background-color: #00A6E0; }

/* Navy Gray - Table headers, footer */
.table-header { background: #212B35; }
.footer { background: #212B35; }

/* Light Gray - Page background */
body { background-color: #F4F4F4; }
```

### Adjust Column Widths

Find the grid template (around line 115):

```css
.attendee-row {
    grid-template-columns: 3fr 1fr 1.5fr 2.5fr;
    /* Name | Table | Theater | Title */
}
```

Modify the proportions as needed (e.g., `4fr 1fr 1fr 3fr`)

### Change Font

Replace Google Fonts link (line 6):

```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font&display=swap">
```

Update font-family (line 13):

```css
body {
    font-family: 'Your Font', sans-serif;
}
```

---

## 🖨️ Printing Instructions

### Quick Print
1. Press `Ctrl+P` (Windows) or `Cmd+P` (Mac)
2. Select your printer
3. Click Print

### Optimal Settings
- **Orientation:** Portrait
- **Page Size:** Letter or A4
- **Margins:** 0.5 inches (all sides)
- **Background Graphics:** Enabled (to show colors)
- **Scale:** 100%

### Print Features
- ✅ Search box automatically hidden
- ✅ Colors optimized for print
- ✅ Page breaks handled properly
- ✅ Headers on each page (if multi-page)

---

## 📱 Mobile Experience

### Automatic Adaptations

**On Small Screens (<768px):**
- Single-column layout for easy scrolling
- Touch-friendly buttons and inputs
- Labels appear on each field
- Larger tap targets
- Optimized font sizes

**Example Mobile View:**
```
Name: Smith, John
Table: 5
Theater: CNA
Title: Senior SC
─────────────────
Name: Doe, Jane
Table: 8
...
```

---

## 🔧 Technical Specifications

### Browser Compatibility
- ✅ Chrome 90+ (Recommended)
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ iOS Safari (iPhone/iPad)
- ✅ Chrome Mobile (Android)

### File Details
- **File Size:** ~22 KB (compressed)
- **Load Time:** <1 second on any connection
- **Language:** HTML5, CSS3, JavaScript (ES6)
- **Font:** Open Sans (Google Fonts CDN)
- **External Dependencies:** Only Google Fonts (gracefully degrades if offline)

### Technology Stack
```
HTML5
├── Semantic markup
├── ARIA labels for accessibility
└── Meta tags for responsive design

CSS3
├── Flexbox for stats
├── CSS Grid for table layout
├── Media queries for responsive design
└── Print-specific styles

JavaScript (ES6)
├── Array methods for filtering
├── DOM manipulation
├── Event listeners for search
└── Template literals for rendering
```

---

## 🛠️ Troubleshooting

### Search Not Working
**Problem:** Search box doesn't filter results  
**Solutions:**
- Ensure JavaScript is enabled in browser
- Clear browser cache (Ctrl+Shift+Delete)
- Try a different browser
- Refresh the page (F5)

### Styling Issues
**Problem:** Page looks unstyled or broken  
**Solutions:**
- Check internet connection (needed for fonts)
- Clear browser cache
- Ensure CSS is loading (view page source)
- Update browser to latest version

### Can't Find Someone
**Problem:** Attendee doesn't appear in search  
**Solutions:**
- Check spelling carefully
- Try partial name (e.g., "smi" instead of "smith")
- Search by table number instead
- Verify they're in the attendee list (view page source)

### Print Quality Issues
**Problem:** Colors don't print correctly  
**Solutions:**
- Enable "Background Graphics" in print settings
- Use "Print to PDF" for digital copies
- Check printer color settings
- Try Chrome/Edge for best print support

---

## 📂 File Structure

```
index.html (Single file containing everything)
│
├── <head>
│   ├── Meta tags (viewport, charset)
│   ├── Title
│   ├── Google Fonts link (Open Sans)
│   └── <style> CSS (embedded)
│       ├── Responsive layout
│       ├── Appian branding
│       ├── Print styles
│       └── Mobile adaptations
│
├── <body>
│   ├── Header (SKO26 title)
│   ├── Stats section (128 attendees, 18 tables)
│   ├── Search box (real-time filtering)
│   ├── Attendee table (grid layout)
│   └── Footer (copyright)
│
└── <script> JavaScript (embedded)
    ├── Attendee data array (128 entries)
    ├── Render function
    └── Search event listener
```

---

## 📝 Version History

### v1.2 (January 16, 2026) - Current
- ✅ Added Campell-Balcombe, Paul to Table 9
- ✅ Updated total attendee count to 128
- ✅ Maintained alphabetical order
- ✅ Verified all data accuracy

### v1.1 (January 2026)
- Updated theater names (CNA, EMEA, USPS, APJ, SPEAR)
- Changed from "Industry" to "Title" (job titles)
- Updated all 127 original attendees
- Maintained same HTML structure

### v1.0 (January 2026)
- Initial release
- Alphabetical directory with search
- Appian branding
- Responsive design
- Print optimization

---

## 👥 Current Attendee List Summary

### By Theater
- **CNA:** 47 attendees across all tables
- **EMEA:** 33 attendees across all tables
- **USPS:** 27 attendees across all tables
- **APJ:** 13 attendees across all tables
- **SPEAR:** 8 attendees across all tables

### By Table (Seats per table)
- **Tables 1, 3, 5:** 8 attendees each
- **Tables 2, 4, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 17, 18:** 7 attendees each
- **Table 15:** 6 attendees

### Recent Addition
- **Campell-Balcombe, Paul** - Table 9, CNA Theater, SC Title

---

## 📞 Support & Contact

### For Event Questions
Contact your SKO26 event coordinator for:
- Seating changes or requests
- Table assignments
- Event logistics

### For Technical Issues
- Open `index.html` in text editor to modify
- All data is plain JavaScript (easy to edit)
- No build process or compilation needed
- Changes take effect immediately

### Need Help?
The file is designed to be self-explanatory:
- View source to see all code
- All comments are included
- Standard web technologies only
- No proprietary formats

---

## 📄 License & Usage

**© 2026 Appian Corporation. All rights reserved.**

This seating chart is created for internal use at the SKO26 (Sales Kickoff 2026) event.

### Permitted Use
- ✅ Internal Appian event use
- ✅ Sharing with event attendees
- ✅ Printing for event signage
- ✅ Mobile access during event
- ✅ Customization for Appian events

### Restrictions
- ❌ External distribution
- ❌ Commercial use
- ❌ Sharing attendee data outside organization

---

## 🎉 Quick Tips

### For Event Organizers
- Deploy to web 1-2 days before event
- Share URL via email/Slack
- Print 2-3 copies for registration desk
- Test search functionality before event
- Have QR code ready for mobile access

### For Attendees
- Bookmark the URL on your phone
- Search your name to find your table
- Search by theater to find colleagues
- Use during event to find people
- Works offline after first load

### For IT/Web Teams
- File is ready for any web server
- No backend or database needed
- Can be hosted on S3, CloudFront, Azure, etc.
- No CORS issues (single file)
- Can add analytics if needed (Google Analytics)

---

## 📊 Statistics

- **Total Lines of Code:** ~380 lines
- **HTML:** ~80 lines
- **CSS:** ~200 lines
- **JavaScript:** ~100 lines
- **Data Entries:** 128 attendees
- **File Size:** 22 KB (uncompressed)
- **Load Time:** <1 second
- **Browser Support:** 99%+ modern browsers

---

**Last Updated:** January 16, 2026  
**Version:** 1.2  
**Attendees:** 128  
**Tables:** 18  
**Status:** ✅ Ready for Production

---

**Questions? Issues? Suggestions?**  
Contact your event coordinator or IT support team.

**Enjoy SKO26! 🎉**
