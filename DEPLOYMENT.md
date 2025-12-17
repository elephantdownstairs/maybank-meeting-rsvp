# GitHub Deployment Instructions

## Step 1: Create GitHub Repository

1. Go to https://github.com and log in
2. Click the "+" icon in the top right → "New repository"
3. Repository name: `maybank-meeting-rsvp` (or any name you prefer)
4. Description: "Meeting RSVP system with Maybank branding"
5. Set to **Public** (required for free GitHub Pages)
6. **DO NOT** initialize with README (we already have one)
7. Click "Create repository"

## Step 2: Push Code to GitHub

Copy and run these commands in your terminal where the files are located:

```bash
git remote add origin https://github.com/YOUR_USERNAME/maybank-meeting-rsvp.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select branch: **main**
5. Click "Save"
6. Wait 1-2 minutes for deployment

## Step 4: Get Your Links

After deployment completes, you'll see:
- **RSVP Form**: `https://YOUR_USERNAME.github.io/maybank-meeting-rsvp/meeting-rsvp.html`
- **Dashboard**: `https://YOUR_USERNAME.github.io/maybank-meeting-rsvp/rsvp-dashboard.html`

## Step 5: Use in Outlook

In your Outlook calendar invitation, add this text:

```
Please confirm your attendance:
👉 RSVP Form: https://YOUR_USERNAME.github.io/maybank-meeting-rsvp/meeting-rsvp.html

This form is required for accurate headcount. Thank you!
```

## Important Notes

⚠️ **Limitation**: Since this uses localStorage, responses are stored in each person's browser. The admin viewing the dashboard will only see responses submitted on their own device.

### To Fix This (Production Use):

You have 3 options:

1. **Simplest**: Just send the form link and manually ask people to screenshot their confirmation
2. **Better**: Use a free form service like Tally.so or Microsoft Forms instead
3. **Best**: Add a backend (requires programming) - I can help with this using:
   - Google Sheets API (free)
   - Firebase (free tier available)
   - Your company's internal API

Would you like help setting up option 3 with a proper backend?

## Troubleshooting

**Problem**: "Permission denied" when pushing
**Solution**: You may need to set up SSH keys or use a Personal Access Token. See: https://docs.github.com/en/authentication

**Problem**: GitHub Pages not working
**Solution**: Make sure repository is Public and wait 5-10 minutes after enabling Pages

**Problem**: Responses not showing in dashboard
**Solution**: This is expected - localStorage is per-browser. See "To Fix This" section above.
