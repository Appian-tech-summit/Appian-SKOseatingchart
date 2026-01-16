# SKO26 Seating Chart - HTML Directory
 
## Overview
 
This is a professional, Appian-branded seating assignment directory for the **SKO26 (Sales Kickoff 2026)** event. The system provides an alphabetical, searchable list of all 128 attendees with their table assignments, theater regions, and job titles.
 
## Features
 
✅ **Alphabetical Directory** - Complete list of all attendees sorted by last name  
✅ **Real-time Search** - Instantly find attendees by name, theater, title, or table number  
✅ **Appian Branding** - Official Appian colors (#00A6E0, #212B35) and Open Sans typography  
✅ **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices  
✅ **Print-Friendly** - Optimized for printing with clean formatting  
✅ **Self-Contained** - Single HTML file with no external dependencies (except Google Fonts)  
✅ **Zero Installation** - Works immediately when opened in any modern browser
 
## Quick Start
 
### Option 1: Open Locally
1. Download `index.html`
2. Double-click to open in your web browser
3. That's it! The seating chart is ready to use
 
### Option 2: Deploy to Web Hosting
To make it accessible via a URL for your event attendees:
 
#### GitHub Pages (Free)
1. Create a new GitHub repository
2. Upload `index.html`
3. Go to Settings → Pages
4. Select "main" branch as source
5. Access at: `https://[username].github.io/[repository-name]`
 
#### Netlify (Free)
1. Visit [netlify.com](https://netlify.com)
2. Drag and drop `index.html` into the deploy area
3. Get instant public URL
4. Share with attendees
 
#### Vercel (Free)
1. Visit [vercel.com](https://vercel.com)
2. Deploy the HTML file
3. Get instant public URL
4. Share with attendees
 
#### Company Web Server
1. Upload `index.html` to your company's web server
2. Share the URL with event attendees
3. Can also host on internal intranet for employee access only
 
## Event Details
 
- **Total Attendees:** 128
- **Tables:** 18 tables (7-8 seats each)
- **Theater Regions:** CNA, EMEA, USPS, APJ, SPEAR
- **Format:** Alphabetical directory with search functionality
 
## Using the Search Feature
 
The search box allows you to instantly filter attendees:
 
- **By Name:** Type "Smith" to find all people with Smith in their name
- **By Theater:** Type "EMEA" to see all EMEA attendees
- **By Title:** Type "Director" to see all Directors
- **By Table:** Type "5" to see all attendees at Table 5
 
**Search is:**
- Case-insensitive
- Real-time (updates as you type)
- Searches across all fields simultaneously
 
## File Structure
 
The `index.html` file contains:
 
1. **HTML Structure** - Semantic markup for the seating directory
2. **CSS Styling** - Appian-branded colors and responsive layout
3. **JavaScript Data** - Array of all 128 attendees with their information
4. **Search Logic** - Real-time filtering functionality
 
## Customization
 
### Updating Attendee Data
 
To modify the attendee list, open `index.html` in a text editor and locate the `attendees` array (around line 255). Each attendee follows this format:
 
```javascript
{name: "Last, First", table: 5, theater: "CNA", title: "Senior SC"}
```
 
**To add a new attendee:**
1. Add a new line in alphabetical order
2. Use the same format as existing entries
3. Save the file
4. Refresh in browser to see changes
 
**To update an attendee:**
1. Find their entry in the `attendees` array
2. Modify the table, theater, or title as needed
3. Save and refresh
 
**To update the total count:**
Update the stat number on line 256:
```html
<div class="stat-number">128</div>
```
 
### Changing Colors
 
Appian brand colors are defined in the CSS section (around line 20). To customize:
 
```css
Primary Blue: #00A6E0
Navy Gray: #212B35
Background: #F4F4F4
```
 
### Modifying Layout
 
The grid layout can be adjusted in the CSS (around line 115):
 
```css
.attendee-row {
    grid-template-columns: 3fr 1fr 1.5fr 2.5fr;
}
```
 
This controls the column widths for: Name | Table | Theater | Title
 
## Browser Compatibility
 
Works in all modern browsers:
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)
 
## Printing Guidelines
 
For best printing results:
 
1. Use **Print to PDF** or a color printer
2. Set orientation to **Portrait**
3. Enable **Background Graphics** for colors
4. Use margins: **0.5 inches** on all sides
 
The design automatically:
- Hides the search box when printing
- Adjusts colors for print media
- Maintains table formatting
 
## Mobile Responsiveness
 
On mobile devices (screens < 768px):
- Grid switches to single-column layout
- Each field is labeled for clarity
- Search remains fully functional
- Touch-friendly buttons and inputs
 
## Technical Details
 
- **File Size:** ~22 KB
- **Load Time:** <1 second on any connection
- **Dependencies:** Google Fonts (Open Sans) - loads from CDN
- **Framework:** Pure HTML/CSS/JavaScript (no libraries required)
- **SEO:** Semantic HTML with proper meta tags
 
## Accessibility
 
The seating chart includes:
- Semantic HTML structure
- Proper ARIA labels
- Keyboard navigation support
- High contrast colors for readability
- Responsive font sizing
 
## Troubleshooting
 
**Search not working:**
- Ensure JavaScript is enabled in your browser
- Try refreshing the page
- Clear browser cache
 
**Page not loading:**
- Check file path is correct
- Ensure HTML file is not corrupted
- Try opening in a different browser
 
**Styling looks wrong:**
- Clear browser cache
- Ensure internet connection for Google Fonts
- Check if browser supports CSS Grid
 
**Can't find an attendee:**
- Check spelling in search box
- Try searching by table number
- Verify attendee is in the data array
 
## Support & Updates
 
For questions or modifications:
- Open the HTML file in any text editor
- All data is stored in plain JavaScript arrays
- No build process or compilation required
- Changes take effect immediately after saving
 
## Version History
 
- **v1.2** (January 16, 2026) - Updated attendee list
  - Added Campell-Balcombe, Paul to Table 9
  - Updated total count to 128 attendees
  - Maintained alphabetical order
 
- **v1.1** (January 2026) - Updated data structure
  - Changed from industries to job titles
  - Updated theater regions (CNA, EMEA, USPS, APJ, SPEAR)
  - Maintained same HTML format
 
- **v1.0** (January 2026) - Initial release
  - Alphabetical seating directory
  - Search functionality
  - Appian branding
  - Responsive design
 
## License
 
© 2026 Appian Corporation. All rights reserved.
 
This seating chart is for internal Appian use at the SKO26 event.
 
## Contact
 
For event questions or seating changes, contact your event coordinator.
