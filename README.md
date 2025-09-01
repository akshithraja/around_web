# Around - Hyperlocal Social Network

A modern, glassmorphism-styled landing page for Around, a location-based social discovery platform. Built with modern web technologies featuring clean monochrome design and interactive elements.

## 🌟 Features

- **Modern Glassmorphism**: Clean white backgrounds with blur effects
- **Monochrome Palette**: Sophisticated black, white, and gray design
- **Responsive Design**: Mobile-first approach that works on all devices
- **Interactive Cards**: Hover highlight effects on feature cards
- **Coming Soon Page**: Email capture functionality for beta access
- **Clean Architecture**: Single HTML file with embedded CSS

## 🎨 Design System

### Colors
- **Primary**: Black (#0A0A0A, #000000)
- **Accent Colors**: 
  - Metallic dark green (#2C5F2D)
  - Metallic dark copper (#B87333)
  - Gold accents (#FFD700)
- **Text**: White/off-white with good contrast
- **Glass Effects**: Semi-transparent whites for glassmorphism

### Typography
- Font Family: System fonts (-apple-system, SF Pro Display style)
- Responsive font sizes using clamp()
- Clear hierarchy with appropriate weights

## 📁 Project Structure

```
around-web/
├── index.html              # Main landing page
├── style.css               # Custom styles and glassmorphism effects  
├── CLAUDE.md              # Development instructions
└── README.md              # This file
```

## 🚀 Getting Started

### Local Development

1. **Clone/Download** the project files
2. **Add Images**: Replace placeholder images in `assets/images/`:
   - `aroundlogo.png` - Company logo
   - `atheev.jpg` - CEO photo
   - `akshith.jpg` - CTO photo
   - `vishnu.jpg` - Design Head photo
3. **Open** `index.html` in your browser or use a local server
4. **Customize** content, colors, and styling as needed

### Using a Local Server (Recommended)

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## 🌐 Deployment to GitHub Pages

### 1. Create GitHub Repository

```bash
git init
git add .
git commit -m "Initial commit: AroundApps website"
git branch -M main
git remote add origin https://github.com/yourusername/aroundapps-website.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repository Settings
2. Scroll to "Pages" section
3. Select Source: "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Save settings

### 3. Custom Domain Setup (Optional)

1. **Add CNAME file** to repository:
```bash
echo "aroundapps.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

2. **Configure DNS** (GoDaddy/your provider):
   - Add A records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Add CNAME record: `www` pointing to `yourusername.github.io`

3. **Enable HTTPS** in GitHub Pages settings

## 📱 Responsive Breakpoints

- **Mobile**: < 480px
- **Tablet**: 481px - 768px
- **Desktop**: > 768px

## ⚡ Performance Features

- **Lazy Loading**: Images load only when needed
- **Passive Event Listeners**: Better scroll performance
- **Reduced Motion**: Respects user accessibility preferences
- **Optimized Animations**: CSS-based animations where possible
- **Efficient DOM Updates**: Throttled scroll events

## 🎯 Browser Support

- Chrome (last 2 versions)
- Firefox (last 2 versions)
- Safari (last 2 versions)
- Edge (last 2 versions)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Customization

### Updating Content

1. **Hero Section**: Edit text in `index.html` around line 50
2. **Features**: Modify feature cards starting around line 70
3. **Founders**: Update founder information around line 140
4. **Form**: Customize form fields around line 200

### Styling Changes

1. **Colors**: Update CSS custom properties in `:root` (main.css line 2-25)
2. **Fonts**: Modify `--font-family-primary` variable
3. **Spacing**: Adjust spacing variables
4. **Animations**: Customize in the animations section (bottom of CSS)

### Adding New Sections

1. Add HTML structure following the existing pattern
2. Use BEM methodology for CSS classes
3. Add corresponding JavaScript if interactivity is needed
4. Update navigation if needed

## 📋 Form Handling

The contact form currently logs data to console. To integrate with a backend:

1. **Update** the `submitForm` method in `main.js`
2. **Replace** the simulation with actual API calls
3. **Add** proper error handling
4. **Consider** services like:
   - Netlify Forms
   - Formspree
   - Custom backend API

## 🔒 Security Considerations

- No sensitive data in client-side code
- Form validation on both client and server side
- Use HTTPS in production
- Regular dependency updates if using build tools

## 📈 Performance Targets

- Lighthouse score > 90
- First Contentful Paint < 1.5s
- Time to Interactive < 3s
- Cumulative Layout Shift < 0.1

## 🐛 Troubleshooting

### Images Not Loading
- Check file paths in `assets/images/`
- Ensure file names match exactly (case-sensitive)
- Verify image formats are web-compatible

### Animations Not Working
- Check if user has reduced motion enabled
- Verify JavaScript is enabled
- Check browser console for errors

### Mobile Menu Issues
- Ensure JavaScript is loaded
- Check viewport meta tag is present
- Verify CSS media queries

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is created for AroundApps. All rights reserved.

## 📞 Support

For questions or support, contact the AroundApps team:
- **CEO**: Atheev Raja
- **CTO**: Akshith Raja  
- **Design Head**: Vishnu M

---

**Built with ❤️ for AroundApps**