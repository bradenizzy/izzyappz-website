# IzzyAppz Website

This is the landing page and Universal Links configuration for the Hands app.

## Structure

```
izzyappz-website/
├── .well-known/
│   └── apple-app-site-association   # iOS Universal Links config
├── r/
│   └── index.html                    # Referral landing page
├── index.html                        # Home page
├── CNAME                             # Custom domain for GitHub Pages
└── README.md
```

## Deployment

This site is deployed via GitHub Pages at: https://www.izzyappz.com

### To Deploy Updates

1. Commit and push changes to the `main` branch
2. GitHub Pages will automatically deploy

## Universal Links

The `apple-app-site-association` file enables iOS Universal Links for:
- Referral links: `https://www.izzyappz.com/r/CODE`

When a user taps a referral link:
1. If app is installed → Opens directly in the app
2. If app is not installed → Shows the referral landing page

## Referral Flow

1. User A shares link: `https://www.izzyappz.com/r/ABC123`
2. User B clicks link
3. Landing page extracts code and copies to clipboard
4. User B downloads app from App Store
5. App reads code from clipboard during account creation
6. Both users get bonus tokens after phone verification
