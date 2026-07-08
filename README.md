# Giridhara VK Sai - Impressive React Portfolio

A stunning, feature-rich React portfolio with Web3Forms integration, animations, theme toggle, and advanced filtering.

## 🌟 Features

### Visual Design
- **Modern Dark Theme** with glassmorphism effects
- **Smooth Animations** using Framer Motion
- **Theme Toggle** (Dark/Light mode)
- **Responsive Design** - Mobile, Tablet, Desktop
- **Gradient Effects** and custom styling

### Functionality
- **Hero Section** with floating avatar animation
- **Stats Dashboard** with animated counters
- **About Section** with personal details
- **Skills Section** with interactive cards and progress bars
- **Projects Showcase** with filtering and search
- **Experience Timeline** with beautiful design
- **Certifications Display** organized by category
- **Achievements Section** with leadership highlights
- **Contact Form** with Web3Forms integration
- **Scroll-to-Top Button** for easy navigation
- **Footer** with social links

### Performance
- **Lazy Loading** for images and components
- **Code Splitting** with Vite
- **Optimized Bundle** size
- **Fast Load Times**

### Web3 Integration
- **Web3Forms** for email delivery
- **Ready for Wallet Connection** (optional future enhancement)

## 🛠️ Tech Stack

- **Frontend**: React 19.2.7
- **Styling**: Tailwind CSS 4.3.2
- **Animations**: Framer Motion 12.42.2
- **Icons**: Lucide React 1.23.0
- **Build Tool**: Vite 8.1.3
- **Email Service**: Web3Forms

## 📦 Installation

### Prerequisites
- Node.js 16+ 
- pnpm (or npm/yarn)

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/gitidhara-portfolio.git
cd gitidhara-portfolio
```

2. **Install dependencies**
```bash
pnpm install
```

3. **Start development server**
```bash
pnpm dev
```

The portfolio will open at `http://localhost:5173`

## 🔧 Configuration

### Update Personal Information

Edit `src/components/Contact.jsx` to update:
- Email address
- Phone number
- Location
- Social media links

### Setup Web3Forms

1. Go to [Web3Forms](https://web3forms.com)
2. Sign up for a free account
3. Create a new form
4. Copy your **Access Key**
5. Update `src/components/Contact.jsx`:

```javascript
body: JSON.stringify({
  access_key: 'YOUR_WEB3FORMS_ACCESS_KEY', // Replace this
  // ... rest of form data
}),
```

### Customize Content

- **Hero Section**: Edit `src/components/Hero.jsx`
- **About Section**: Edit `src/components/About.jsx`
- **Skills**: Edit `src/components/Skills.jsx`
- **Projects**: Edit `src/components/Projects.jsx`
- **Experience**: Edit `src/components/Experience.jsx`
- **Certifications**: Edit `src/components/Certifications.jsx`
- **Achievements**: Edit `src/components/Achievements.jsx`

## 🚀 Deployment

### Option 1: Vercel (Recommended)

1. **Push to GitHub**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/gitidhara-portfolio.git
git push -u origin main
```

2. **Deploy to Vercel**
   - Go to [Vercel](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy"
   - Your portfolio is live! 🎉

### Option 2: Netlify

1. **Build the project**
```bash
pnpm build
```

2. **Deploy to Netlify**
   - Go to [Netlify](https://netlify.com)
   - Drag and drop the `dist` folder
   - Your portfolio is live! 🎉

### Option 3: GitHub Pages

1. **Update vite.config.js**
```javascript
export default defineConfig({
  base: '/gitidhara-portfolio/', // Replace with your repo name
  plugins: [react()],
})
```

2. **Build and deploy**
```bash
pnpm build
git add dist
git commit -m "Deploy to GitHub Pages"
git push
```

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages"
   - Set source to `gh-pages` branch

## 📁 Project Structure

```
src/
├── components/
│   ├── Header.jsx           # Navigation & theme toggle
│   ├── Hero.jsx             # Hero section
│   ├── Stats.jsx            # Stats dashboard
│   ├── About.jsx            # About section
│   ├── Skills.jsx           # Skills with progress bars
│   ├── Projects.jsx         # Projects with filter & search
│   ├── Experience.jsx       # Experience timeline
│   ├── Certifications.jsx   # Certifications display
│   ├── Achievements.jsx     # Achievements section
│   ├── Contact.jsx          # Contact form with Web3Forms
│   ├── Footer.jsx           # Footer
│   └── ScrollToTop.jsx      # Scroll to top button
├── hooks/
│   └── useInView.js         # Intersection observer hook
├── App.jsx                  # Main app component
├── index.css                # Global styles
└── main.jsx                 # Entry point
```

## 🎨 Customization

### Colors

Edit `tailwind.config.js` to change the color scheme:

```javascript
theme: {
  extend: {
    colors: {
      primary: "#00bcd4",      // Cyan
      secondary: "#0077ff",    // Blue
      dark: "#0d1117",         // Dark background
      card: "#161b22",         // Card background
      // ... more colors
    },
  },
}
```

### Fonts

The portfolio uses **Poppins** font from Google Fonts. To change:

1. Update `src/index.css`
2. Change the font import
3. Update `tailwind.config.js` font family

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 🔐 Security

- No sensitive data stored in code
- Web3Forms handles email securely
- Environment variables for sensitive data

## 📝 License

This portfolio template is open source and available under the MIT License.

## 🤝 Contributing

Feel free to fork, modify, and use this portfolio for your own projects!

## 📧 Contact

For questions or support, reach out through the contact form on the portfolio.

## 🙏 Acknowledgments

- [React](https://react.dev)
- [Tailwind CSS](https://tailwindcss.com)
- [Framer Motion](https://www.framer.com/motion)
- [Vite](https://vitejs.dev)
- [Web3Forms](https://web3forms.com)

---

**Made with ❤️ using React, Tailwind CSS, and Framer Motion**
