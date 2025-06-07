# MOOLI IVAN - LC5 Chairperson Campaign Website

A professional campaign website for MOOLI IVAN's candidacy for LC5 Chairperson of Manafwa District (2026-2031) under the Alliance for National Transformation (ANT) party.

## 🚀 Features

- **Responsive Design**: Mobile-first approach that works on all devices
- **Modern UI/UX**: Clean, professional design with ANT party colors (Purple, Orange, White)
- **Complete Campaign Package**: All essential sections for a political campaign
- **Interactive Elements**: Forms, gallery lightbox, smooth scrolling
- **SEO Optimized**: Proper meta tags and semantic HTML structure
- **Performance Optimized**: Lazy loading, debounced scroll events, image preloading

## 📁 Project Structure

```
mooliivan/
├── index.html              # Main HTML file
├── styles.css              # Complete CSS styling
├── script.js               # JavaScript functionality
├── MOOLIIVAN.JPG          # Candidate photo
├── Alliance_for_National_Transformation.png  # Party logo
└── README.md              # This file
```

## 🎨 Design Features

### Color Scheme (ANT Party Colors)
- **Primary Purple**: #6B46C1 (ANT party primary color)
- **Secondary Orange**: #F97316 (ANT party accent color)
- **White**: #FFFFFF (Clean backgrounds)
- **Supporting colors**: Various shades of gray for text and backgrounds

### Sections Included
1. **Homepage**: Hero section with candidate photo and call-to-action
2. **About**: Leadership experience, education, and community service
3. **Manifesto**: Six key areas of focus for district development
4. **News & Updates**: Latest campaign activities and announcements
5. **Gallery**: Photo gallery with lightbox functionality
6. **Join Us**: Volunteer signup form with local sub-county options
7. **Donate**: Campaign contribution information
8. **Contact**: Contact form and office information

## 🛠️ Setup & Usage

### Quick Start
1. Ensure you have the candidate photo (`MOOLIIVAN.JPG`) and party logo (`Alliance_for_National_Transformation.png`) in the root directory
2. Open `index.html` in a web browser
3. The website is ready to use!

### For Web Hosting
1. Upload all files to your web hosting provider
2. Ensure the domain points to the directory containing `index.html`
3. The website will be live at your domain

## ✏️ Customization Guide

### Adding Your Own Content

#### 1. Update Contact Information
In `index.html`, search for and replace:
- Phone numbers: `+256-XXX-XXXXXX`
- Email: `info@mooliivanmanafwa.com`
- Bank details in the donate section

#### 2. Add Real News Articles
Replace the sample news items in the news section with actual campaign updates.

#### 3. Update Gallery Images
Replace the sample gallery images with actual campaign photos. Ensure all images are optimized for web (under 500KB each).

#### 4. Customize Sub-counties
In the volunteer form, update the sub-county options to match Manafwa District's actual sub-counties:
```html
<option value="manafwa">Manafwa</option>
<option value="bulegeni">Bulegeni</option>
<option value="malaba">Malaba</option>
<option value="bukigai">Bukigai</option>
<option value="tsima">Tsima</option>
```

#### 5. Add Social Media Links
Update the social media links in the contact and footer sections with actual social media profiles.

### Technical Customizations

#### Changing Colors
Update the CSS variables in `styles.css`:
```css
:root {
    --primary-purple: #6B46C1;
    --secondary-orange: #F97316;
    --accent-white: #FFFFFF;
    /* ... other colors */
}
```

#### Adding New Sections
1. Add the HTML structure in `index.html`
2. Add corresponding styles in `styles.css`
3. Update the navigation menu to include the new section

## 📱 Mobile Responsiveness

The website is fully responsive and includes:
- Mobile-friendly navigation with hamburger menu
- Optimized layouts for tablets and phones
- Touch-friendly buttons and forms
- Properly scaled images and text

## 🔧 Form Handling

### Current Implementation
The forms are set up with JavaScript validation and display success/error messages. Currently, they:
- Validate required fields
- Check email format
- Validate Ugandan phone numbers
- Show confirmation messages

### For Production Use
To make the forms functional, you'll need to:

1. **Set up a backend server** (PHP, Node.js, Python, etc.)
2. **Configure email sending** (SMTP, SendGrid, etc.)
3. **Add database storage** for volunteer and contact submissions
4. **Update the JavaScript** to send data to your backend

Example backend endpoint update in `script.js`:
```javascript
// Replace the console.log with actual API call
fetch('/api/volunteer', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(data)
})
.then(response => response.json())
.then(result => {
    showMessage('Thank you for joining our movement!', 'success');
});
```

## 🌐 SEO Optimization

The website includes:
- Proper meta tags for search engines
- Semantic HTML structure
- Alt text for images
- Descriptive page title and description
- Open Graph tags for social media sharing

## ⚡ Performance Features

- **Image Optimization**: Lazy loading for non-critical images
- **Code Optimization**: Minified CSS and JavaScript
- **Caching**: Proper cache headers recommended for production
- **CDN Ready**: External resources (fonts, icons) loaded from CDNs

## 🚀 Deployment Options

### 1. Static Web Hosting
- **Netlify**: Free hosting with automatic deployments
- **Vercel**: Free hosting with excellent performance
- **GitHub Pages**: Free hosting if code is on GitHub

### 2. Traditional Web Hosting
- Upload files via FTP to any web hosting provider
- Ensure PHP support if adding backend functionality

### 3. Content Management
- Can be integrated with WordPress or other CMS
- Convert to dynamic templates for easy content updates

## 📊 Analytics & Tracking

To track website performance, add:
- Google Analytics code before closing `</head>` tag
- Facebook Pixel for social media advertising
- Campaign-specific tracking parameters

## 🔒 Security Considerations

For production deployment:
- Use HTTPS (SSL certificate)
- Implement CSRF protection for forms
- Sanitize all user inputs
- Regular security updates

## 📞 Support & Maintenance

### Regular Updates Needed
- News and events section
- Gallery with new campaign photos
- Contact information if office location changes
- Social media links and content

### Technical Maintenance
- Regular backup of website files
- Monitor website performance and uptime
- Update dependencies and security patches

## 📄 License & Credits

This website template is created specifically for MOOLI IVAN's campaign. The design incorporates:
- Alliance for National Transformation party branding
- Ugandan political context and cultural considerations
- Local government structure (LC5, sub-counties)

---

**Developed for MOOLI IVAN Campaign 2026**  
*"Change You Can Trust"*

For technical support or customization requests, please contact the development team. 