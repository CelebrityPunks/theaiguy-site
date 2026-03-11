# AI Consultant Landing Page

Your personal landing page for Facebook ads and lead generation.

## Quick Setup

### 1. Add Your Photo
Save a professional photo as `photo.jpg` in this folder. Recommended:
- Square crop (1:1 ratio)
- At least 300x300px
- Professional but approachable (smile!)

### 2. Update Phone Number
In `index.html`, find and replace:
```
+1XXXXXXXXXX → your actual number (e.g., +16195551234)
+1 (XXX) XXX-XXXX → formatted display (e.g., +1 (619) 555-1234)
```

Search for "XXXXXXXXXX" to find all instances.

### 3. Update WhatsApp Link
Find the WhatsApp link and update the number:
```
https://wa.me/1XXXXXXXXXX → https://wa.me/16195551234
```

### 4. Update Location (Optional)
Find "San Diego, CA" and change to your actual location.

## Deploy Options

### Option A: Netlify (Easiest - Free)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop this folder
3. Get a free URL like `yourname.netlify.app`
4. Optional: Connect custom domain

### Option B: Vercel (Free)
```bash
npm i -g vercel
cd landing-page
vercel
```

### Option C: GitHub Pages (Free)
1. Create GitHub repo
2. Push this folder
3. Settings → Pages → Enable
4. Get URL like `yourusername.github.io/repo-name`

### Option D: Custom Domain + Hosting
Any web host works - it's just HTML/CSS.

## Facebook Ads Setup

### 1. Create Facebook Pixel
1. Go to [Facebook Business Suite](https://business.facebook.com)
2. Events Manager → Connect Data Sources → Web
3. Create Pixel → Copy the code

### 2. Add Pixel to Page
In `index.html`, find this comment and replace with your pixel code:
```html
<!-- Facebook Pixel placeholder -->
<!-- <script>!function(f,b,e,v,n,t,s)...</script> -->
```

### 3. Test Pixel
- Install [Facebook Pixel Helper](https://chrome.google.com/webstore/detail/facebook-pixel-helper) Chrome extension
- Visit your page
- Verify pixel fires on page load and phone reveal

### 4. Create Ad Campaign
**Objective:** Lead Generation or Traffic
**Audience suggestions:**
- Age: 35-65
- Interests: Small business, entrepreneurship, business owner
- Behaviors: Small business owners, engaged shoppers
- Location: Your service area (or nationwide)

**Ad Copy Template:**
```
Tired of missing calls and losing customers?

AI can answer your phone 24/7, capture leads, and book appointments — even while you sleep.

I help small business owners implement simple AI tools that actually work.

📞 Free 15-min consultation
No tech jargon. No sales pitch. Just solutions.

[Learn More]
```

## Tracking Conversions

The page tracks these events:
- **Page View** - When someone lands on the page
- **Contact** - When someone reveals the phone number

These fire to Facebook Pixel automatically if installed.

## Customization Ideas

### Change Colors
Find this line and modify the gradient:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

Color suggestions:
- Professional blue: `#2563eb` to `#1e40af`
- Trust green: `#059669` to `#047857`
- Bold orange: `#f97316` to `#ea580c`

### Add Testimonials
Once you have clients, add a testimonials section before the CTA.

### Add Calendly
Instead of phone reveal, embed Calendly:
```html
<a href="https://calendly.com/yourname/15min" class="btn btn-primary">
    📅 Book Free Call
</a>
```

## File Structure
```
landing-page/
├── index.html    # Main page
├── photo.jpg     # Your photo (add this)
└── README.md     # This file
```

## Next Steps

1. [ ] Add your photo
2. [ ] Update phone number
3. [ ] Deploy to Netlify/Vercel
4. [ ] Set up Facebook Pixel
5. [ ] Create test ad ($5-10/day)
6. [ ] Monitor and iterate
