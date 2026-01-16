# FreeCash Landing Page - RewardOrbit

## 🚀 Quick Setup

1. Upload all files to your web host
2. Use this URL in TikTok ads: `https://yourdomain.com/?utm_campaign={{campaign.name}}`

## 🔗 Your Affiliate Link

**RewardOrbit Link:** 
```
https://rewardorbit.com/r/eyJ0IjoiZnJlZWNhc2gtY3BpIiwidSI6IjY5NjM1OTE2MTFjOTZjMzMzNDEzMWJjYSIsInRzIjoxNzY4NjA1MTU2MTA2fQ?s2=
```

**Example with SubID:**
```
https://rewardorbit.com/r/eyJ0IjoiZnJlZWNhc2gtY3BpIiwidSI6IjY5NjM1OTE2MTFjOTZjMzMzNDEzMWJjYSIsInRzIjoxNzY4NjA1MTU2MTA2fQ?s2=tiktok_jan_v1
```

## 📊 How It Works

1. **TikTok Ad URL:** `https://yourdomain.com/?utm_campaign=tiktok_jan_v1`
2. User lands on page
3. Clicks "Download App" button
4. TikTok pixel fires 2 events
5. **Redirects to:** `https://rewardorbit.com/r/...?s2=tiktok_jan_v1`

## 🎯 SubID Parameter Support

Priority order (checks top to bottom):
1. **s2=** (your RewardOrbit link uses this)
2. **s1=** (fallback support)
3. source_id=
4. source=

To switch parameters, just change the link in index.html and it will auto-detect!

## 🎪 TikTok Pixel

**Pixel ID:** `D4DHBLBC77UCD4LE0TM0`

**Events on button click:**
- CompletePayment ($0.50 value)
- CompleteRegistration ($0.50 value)

**Note:** 1 click = 2 conversion events in TikTok (this is normal!)

## 📱 Files Included

- `index.html` - Main landing page
- `logo.jpg` - FreeCash logo
- `events.js` - TikTok pixel
- `inter-font.css` - Font file
- `backblue.gif` - Background
- `fade.gif` - Fade effect
- `README.md` - This file

## ✅ Testing

1. Visit: `https://yourdomain.com/?utm_campaign=test`
2. Click "Download App" button
3. Verify redirect URL has `?s2=test`

## 🔧 Changing the Link

To use a different affiliate link, edit `index.html` line with:
```html
<a href="YOUR_LINK_HERE?s2=" class="cta-btn" id="mainBtn">
```

Or use `?s1=` if your new link needs s1 parameter - the code supports both!
