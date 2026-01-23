# AV Window Tinting Website

Professional window tinting services for the Antelope Valley (Palmdale, Lancaster, Quartz Hill).

## 🌐 Live Site
- **CloudFront URL**: https://d33vnaateyj3z0.cloudfront.net/
- **Custom Domain**: (To be configured)

## 🏗️ Site Architecture

### Hosting Infrastructure
- **Storage**: AWS S3 Bucket
- **CDN**: AWS CloudFront Distribution
- **Deployment**: GitHub Actions (automated sync on push to main)
- **Repository**: https://github.com/Dronesmiths/AV-Window-Tinting

### Technology Stack
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Images**: WebP format (85% quality)
- **Fonts**: Google Fonts (Inter)
- **Theme**: Professional blue (#1e3a8a, #3b82f6)

## 📁 Project Structure

```
AV-Window-Tinting/
├── index.html              # Main homepage
├── css/
│   └── styles.css         # Global styles with blue theme
├── js/
│   └── script.js          # Interactive components (slider, mobile nav)
├── images/                # All WebP optimized images
│   ├── hero-home.webp     # Hero: Brian tinting car window
│   ├── brian-uniform.webp # About: Brian headshot
│   ├── service-*.webp     # 6 service card images
│   ├── before.webp        # Before/after slider
│   └── after.webp
├── .github/
│   └── workflows/
│       └── deploy.yml     # Auto-deploy to S3 on push
└── README.md              # This file
```

## 🎨 Services Offered

1. **Residential Tinting** - Home window films for energy savings
2. **Commercial Tinting** - Office and retail building films
3. **Automotive Tinting** - Car, truck, SUV window tinting
4. **Security Film** - Shatter-resistant protective films
5. **Decorative Film** - Frosted and etched privacy films
6. **Heat Rejection Film** - Ceramic films blocking 80% solar heat

## 🚀 Local Development

### Start Local Server
```bash
cd /Users/mediusa/NOVA/Repos/AV-Window-Tinting
python3 -m http.server 8001
```

Then open: http://localhost:8001

### Deploy to Production
Simply push to the `main` branch:
```bash
git add .
git commit -m "Your changes"
git push origin main
```

GitHub Actions will automatically sync to S3 and invalidate CloudFront cache.

## 📝 Recent Changes (Jan 2026)

### Brand Transformation
- ✅ Converted from "AV Tree Pros" to "AV Window Tinting"
- ✅ Updated all branding, colors, and content
- ✅ Implemented professional blue theme (#1e3a8a, #3b82f6)

### Image Optimization
- ✅ Generated 6 professional service images (residential, commercial, automotive, security, decorative, heat rejection)
- ✅ Converted all PNG images to WebP format (average 82% file size reduction)
- ✅ Updated hero image to Brian tinting car window
- ✅ Updated owner photo to Brian's professional headshot
- ✅ Removed all unused tree service images (31 files deleted)

### Content Updates
- ✅ Updated all service descriptions for window tinting
- ✅ Updated meta tags and SEO content
- ✅ Updated schema.org structured data
- ✅ Updated contact information and CTAs

### Technical Improvements
- ✅ WebP image format for 82% smaller file sizes
- ✅ Optimized hero background image
- ✅ Clean file structure (removed unused services directory)
- ✅ Updated CSS references for WebP images

## 📞 Contact Information

- **Business**: AV Window Tinting
- **Phone**: (661) 555-TINT
- **Owner**: Brian
- **Service Area**: Palmdale, Lancaster, Quartz Hill, Antelope Valley

## 🔧 Maintenance

### Image Conversion (PNG to WebP)
```bash
cwebp -q 85 input.png -o output.webp
```

### Bulk Image Conversion
```bash
for file in images/*.png; do cwebp -q 85 "$file" -o "${file%.png}.webp"; done
```

### Update HTML References
```bash
sed -i '' 's/\.png/.webp/g' index.html
```

## 📊 Performance Metrics

- **Total Images**: 10 WebP files
- **Total Image Size**: ~1.5MB (down from ~7.5MB PNG)
- **Compression**: 82% average reduction
- **Page Load**: Optimized for fast loading

## 🎯 SEO Strategy

- Local business schema markup
- Service-specific meta descriptions
- Geo-targeted keywords (Palmdale, Lancaster, Antelope Valley)
- Mobile-responsive design
- Fast loading times with WebP images
- Clean URL structure

---

**Last Updated**: January 22, 2026
**Maintained by**: AI Pilots (Brian Smith)
