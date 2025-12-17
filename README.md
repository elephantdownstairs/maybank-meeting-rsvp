# Meeting RSVP System

A simple, professional RSVP system for tracking meeting attendance with Maybank corporate branding.

## Features

- ✅ Clean, professional form with Maybank yellow/black theme
- ✅ Automatic duplicate prevention (same name + email overwrites old response)
- ✅ Real-time dashboard with statistics
- ✅ Export responses to CSV
- ✅ Mobile responsive design
- ✅ No backend required (uses localStorage)

## Files

- **meeting-rsvp.html** - The RSVP form that attendees fill out
- **rsvp-dashboard.html** - Admin dashboard to view and manage responses

## How to Use

### For Meeting Organizers:

1. Host both HTML files on a web server or GitHub Pages
2. Share the `meeting-rsvp.html` link in your Outlook calendar invitation
3. Open `rsvp-dashboard.html` to track responses in real-time

### For Attendees:

1. Click the RSVP link from the meeting invitation
2. Fill in your name and work email
3. Select your response (Yes/No/Maybe)
4. Add any comments (optional)
5. Submit

## Deployment Options

### Option 1: GitHub Pages (Recommended)
1. Push this repository to GitHub
2. Go to Settings → Pages
3. Select branch `main` and folder `/root`
4. Your forms will be live at `https://yourusername.github.io/repository-name/`

### Option 2: Company Intranet
Upload both HTML files to your company's file server or intranet

### Option 3: Local Network
Host on any web server accessible to meeting participants

## Technical Details

- **Storage**: Browser localStorage (responses persist per browser)
- **Font**: Poppins (Google Fonts)
- **Colors**: Maybank Yellow (#FFC107) and Black (#000000)
- **Framework**: Pure HTML/CSS/JavaScript (no dependencies)

## Customization

To customize the form:
- Update meeting details in the header section
- Modify colors in the CSS section
- Add additional form fields as needed

## Notes

- Responses are stored locally in the browser
- For production use with multiple admins, consider integrating a backend API
- Same person (name + email) submitting twice will overwrite their previous response
- Dashboard auto-refreshes every 30 seconds

## License

Free to use and modify for internal company purposes.
