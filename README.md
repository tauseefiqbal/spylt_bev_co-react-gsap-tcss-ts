# Spylt - Premium Beverage Landing Page

A stunning, interactive landing page for Spylt beverage company built with React, TypeScript, and GSAP animations. Experience smooth scrolling, engaging video content, and immersive storytelling.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Deployment](#deployment)
- [Test and Admin Users Credentials](#test-and-admin-users-credentials)
- [How to Use App for Regular User](#how-to-use-app-for-regular-user)
- [How to Use App for Admin User](#how-to-use-app-for-admin-user)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Development](#development)
- [Building for Production](#building-for-production)
- [Environment Variables](#environment-variables)
- [Browser Support](#browser-support)
- [Performance Optimization](#performance-optimization)
- [Contributing](#contributing)
- [License](#license)

---

## Features

✅ **Smooth Scroll Experience** - GSAP ScrollSmoother provides buttery-smooth scrolling throughout the entire page

✅ **Video Background Hero** - Stunning full-screen video background with animated title text

✅ **Interactive Flavor Showcase** - Explore 6 delicious milk flavors (Chocolate, Strawberry, Cookies & Cream, Peanut Butter Chocolate, Vanilla, Max Chocolate)

✅ **Scroll-Triggered Animations** - Text and elements animate into view as you scroll using GSAP ScrollTrigger

✅ **Character-by-Character Text Animation** - Beautiful text reveals using GSAP SplitText for individual character animations

✅ **Hover-to-Play Video Testimonials** - Interactive video cards that play on hover with 7 customer testimonials

✅ **Pinned Video Section** - Scroll-controlled video with circular reveal animation effect

✅ **Nutrition Information Display** - Clear presentation of key nutritional benefits (Potassium, Calcium, Vitamins A & D, Iron)

✅ **Fully Responsive Design** - Optimized for desktop, tablet, and mobile devices using Tailwind CSS

✅ **Custom Font Integration** - Antonio (Google Fonts) and ProximaNova for premium typography

✅ **Type-Safe Codebase** - Built with TypeScript for enhanced code quality and developer experience

✅ **Optimized Video Preloading** - Smart video preloading strategy for smooth playback without blocking page load

✅ **Brand Messaging Sections** - Engaging storytelling with scroll-based color transitions

✅ **Modern ES2020+ JavaScript** - Leveraging the latest ECMAScript features

✅ **Fast Development with Vite** - Lightning-fast HMR (Hot Module Replacement) for instant updates

---

## Tech Stack

### Frontend Framework
- **React 19.2.0** - Modern UI library with latest features
- **TypeScript 5.7.2** - Type-safe JavaScript for better code quality

### Build Tool
- **Vite 7.3.1** - Next-generation frontend tooling with instant HMR

### Animation Library
- **GSAP (GreenSock) 3.12.7 Trial** - Professional-grade animation platform
  - ScrollTrigger - Scroll-based animations
  - ScrollSmoother - Smooth scrolling effect
  - SplitText - Text splitting for character animations
- **@gsap/react 2.1.2** - React integration hooks

### Styling
- **Tailwind CSS 4.2.0** - Utility-first CSS framework
- **PostCSS 8.5.2** - CSS transformations

### Responsive Design
- **react-responsive 10.0.1** - Media query hooks for React

### Development Tools
- **ESLint 9.20.0** - Code linting
- **@vitejs/plugin-react 4.3.4** - React Fast Refresh support

### Fonts
- **Antonio** (Google Fonts) - Display headings
- **Proxima Nova Regular** (Local) - Body text

---

## Deployment

### Live Application

🚀 **APP URL**: [Your Live URL Here]

### Deployment Platforms

This application can be deployed to:

- **Vercel** (Recommended for Vite projects)
  ```bash
  npm run build
  vercel --prod
  ```

- **Netlify**
  ```bash
  npm run build
  # Deploy dist/ folder
  ```

- **GitHub Pages**
  ```bash
  npm run build
  # Deploy dist/ folder to gh-pages branch
  ```

- **Azure Static Web Apps**
  ```bash
  npm run build
  # Deploy using Azure CLI or GitHub Actions
  ```

### Build Command
```bash
npm run build
```

### Output Directory
```
dist/
```

---

## Test and Admin Users Credentials

> **Note**: This is a static landing page without authentication. No login credentials are required.

### Regular User Access
- **Access Level**: Public
- **Authentication**: None required
- **Permissions**: View all content, interact with videos and animations

### Admin User Access
- **Access Level**: Not applicable
- **Authentication**: Not implemented
- **Permissions**: N/A

*For a production application with user management, implement authentication using services like:*
- Firebase Authentication
- Auth0
- Azure AD B2C
- Custom JWT-based auth

---

## How to Use App for Regular User

### Accessing the Application

1. **Open the Application**
   - Navigate to the live URL in your web browser
   - Recommended browsers: Chrome, Firefox, Safari, Edge (latest versions)

2. **Scroll Through Sections**
   - Use your mouse wheel, trackpad, or touch gestures to scroll
   - Experience smooth scrolling powered by GSAP ScrollSmoother

### Exploring Features

3. **Hero Section**
   - Watch the full-screen video background
   - See animated title text reveal character by character

4. **Brand Message**
   - Scroll through the messaging sections
   - Watch text colors animate as you scroll

5. **Flavor Showcase**
   - View all 6 available milk flavors
   - See product images and flavor names
   - Note the rotation animations on desktop

6. **Nutrition Information**
   - Learn about key nutritional benefits
   - See detailed amounts for each nutrient

7. **Benefits Section**
   - Discover product advantages
   - Experience scroll-triggered content reveals

8. **Video Testimonials**
   - Hover over customer cards to play their video testimonials
   - See 7 different customer experiences
   - Move your mouse away to pause the video

9. **Pinned Video Section**
   - Scroll to trigger the circular reveal animation
   - Watch the video expand from a circle to full screen

10. **Footer**
    - View brand information and splash video animation

### Mobile Experience

- **Touch Gestures**: Swipe to scroll
- **Video Interaction**: Tap testimonial cards to play (auto-pause on scroll)
- **Responsive Layout**: Optimized for all screen sizes
- **Performance**: Optimized video loading for mobile networks

---

## How to Use App for Admin User

> **Note**: This is a static landing page without an admin panel. Content management requires direct code/file updates.

### Content Management

To update content as an administrator/developer:

1. **Update Flavors**
   - Edit `src/constants/index.ts`
   - Modify the `flavorlists` array
   - Update images in `public/images/`

2. **Update Nutrition Data**
   - Edit `src/constants/index.ts`
   - Modify the `nutrientLists` array

3. **Update Testimonials**
   - Edit `src/constants/index.ts`
   - Modify the `cards` array
   - Add/replace videos in `public/videos/`

4. **Update Videos**
   - Replace video files in `public/videos/`
   - Supported formats: MP4 (recommended)
   - Keep similar aspect ratios for best results

5. **Update Styling**
   - Edit component files in `src/sections/` and `src/components/`
   - Modify Tailwind classes for design changes
   - Update `tailwind.config.js` for theme customization

6. **Deploy Changes**
   ```bash
   npm run build
   # Deploy dist/ folder to your hosting platform
   ```

### Future Admin Panel Considerations

For a full CMS admin panel, consider integrating:
- **Headless CMS**: Sanity, Contentful, Strapi
- **Static Site CMS**: NetlifyCMS, TinaCMS
- **Custom Admin Dashboard**: React Admin, Refine

---

## Project Structure

```
spylt_bev_co/
├── public/
│   ├── fonts/
│   │   └── ProximaNova-Regular.otf
│   ├── images/
│   │   └── [Product and testimonial images]
│   └── videos/
│       ├── hero-bg.mp4
│       ├── pin-video.mp4
│       ├── splash.mp4
│       └── f1.mp4 - f7.mp4 (testimonials)
├── src/
│   ├── components/
│   │   ├── ClipPathTitle.tsx
│   │   ├── FlavorSlider.tsx
│   │   ├── FlavorTitle.tsx
│   │   ├── NavBar.tsx
│   │   └── VideoPinSection.tsx
│   ├── sections/
│   │   ├── BenefitSection.tsx
│   │   ├── FlavorSection.tsx
│   │   ├── FooterSection.tsx
│   │   ├── HeroSection.tsx
│   │   ├── MessageSection.tsx
│   │   ├── NutritionSection.tsx
│   │   └── TestimonialSection.tsx
│   ├── constants/
│   │   └── index.ts (Type definitions and data)
│   ├── App.tsx (Main component)
│   ├── main.tsx (Entry point)
│   └── index.css (Global styles)
├── index.html (Vite entry HTML)
├── tsconfig.json (TypeScript config)
├── tsconfig.node.json (Node TypeScript config)
├── vite.config.ts (Vite configuration)
├── tailwind.config.js (Tailwind CSS config)
├── postcss.config.js (PostCSS config)
├── eslint.config.js (ESLint config)
└── package.json (Dependencies)
```

---

## Installation

### Prerequisites

- **Node.js**: v18.0.0 or higher
- **npm**: v9.0.0 or higher (or yarn/pnpm)

### Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd spylt_bev_co
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Verify installation**
   ```bash
   npm list
   ```

---

## Development

### Start Development Server

```bash
npm run dev
```

The application will start on `http://localhost:5173` (or next available port).

### Development Features

- **Hot Module Replacement (HMR)**: Instant updates without full page reload
- **TypeScript Type Checking**: Real-time type errors in your IDE
- **Fast Refresh**: React component state preserved during updates
- **Source Maps**: Debug original TypeScript code in browser DevTools

### Useful Commands

```bash
# Run development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linter
npm run lint

# Type check without building
npx tsc --noEmit
```

---

## Building for Production

### Build Command

```bash
npm run build
```

### Output

- Production-optimized files in `dist/` folder
- Minified JavaScript and CSS
- Optimized assets (images, videos)
- Source maps for debugging

### Preview Production Build

```bash
npm run preview
```

Serves the `dist/` folder at `http://localhost:4173`

### Production Optimization

- **Code Splitting**: Automatic chunk splitting for optimal loading
- **Tree Shaking**: Removes unused code
- **Asset Optimization**: Compressed images and videos
- **CSS Purging**: Removes unused Tailwind CSS classes
- **Lazy Loading**: Videos load on-demand

---

## Environment Variables

Currently, this project does not use environment variables. For future API integrations:

1. Create `.env` file:
   ```env
   VITE_API_URL=https://api.example.com
   VITE_GA_ID=G-XXXXXXXXXX
   ```

2. Access in code:
   ```typescript
   const apiUrl = import.meta.env.VITE_API_URL;
   ```

3. Update `.gitignore`:
   ```
   .env
   .env.local
   ```

---

## Browser Support

### Fully Supported

- ✅ Chrome 90+ (Windows, macOS, Linux, Android)
- ✅ Firefox 88+ (Windows, macOS, Linux)
- ✅ Safari 14+ (macOS, iOS)
- ✅ Edge 90+ (Windows, macOS)

### Partially Supported

- ⚠️ Chrome 85-89 (Some GSAP features may have degraded performance)
- ⚠️ Safari 13 (Video autoplay may require user interaction)

### Not Supported

- ❌ Internet Explorer (all versions)
- ❌ Browsers without ES2020 support

### Required Browser Features

- ES2020+ JavaScript
- CSS Grid & Flexbox
- Video element with autoplay
- Intersection Observer API
- CSS clip-path
- CSS transforms

---

## Performance Optimization

### Current Optimizations

1. **Font Loading**
   - GSAP animations wait for `document.fonts.ready`
   - Prevents layout shifts and incorrect text measurements

2. **Video Strategy**
   - `preload="auto"` for hero and footer videos
   - Lazy loading for testimonial videos (play on hover)
   - `muted` and `playsInline` for autoplay compatibility

3. **Code Splitting**
   - Dynamic imports for routes (if implemented)
   - Vite automatic chunking

4. **Image Optimization**
   - Use WebP format for better compression (recommended)
   - Add responsive images with `srcset`

### Recommended Improvements

```typescript
// Lazy load GSAP plugins
const ScrollTrigger = await import('gsap/ScrollTrigger');

// Image lazy loading
<img loading="lazy" src="image.jpg" alt="..." />

// Intersection Observer for components
const [isVisible, setIsVisible] = useState(false);
useEffect(() => {
  const observer = new IntersectionObserver(entries => {
    if (entries[0].isIntersecting) setIsVisible(true);
  });
  observer.observe(ref.current);
}, []);
```

---

## Contributing

### Getting Started

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes
4. Commit with descriptive messages: `git commit -m 'Add amazing feature'`
5. Push to your branch: `git push origin feature/amazing-feature`
6. Open a Pull Request

### Code Standards

- **TypeScript**: All new code must be TypeScript
- **ESLint**: Follow the ESLint configuration
- **Formatting**: Use Prettier (recommended)
- **Commits**: Use conventional commit messages

### Pull Request Guidelines

- Describe your changes clearly
- Include screenshots/videos for UI changes
- Test on multiple browsers
- Update documentation if needed
- Ensure all tests pass

---

## License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2026 Spylt

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## Contact & Support

- **Project Repository**: [GitHub URL]
- **Issues**: [GitHub Issues URL]
- **Discussions**: [GitHub Discussions URL]
- **Email**: support@spylt.com

---

## Acknowledgments

- **GSAP (GreenSock)** - For the amazing animation platform
- **Vite Team** - For the lightning-fast build tool
- **React Team** - For the powerful UI library
- **Tailwind CSS** - For the utility-first CSS framework

---

Made with ❤️ by the Spylt Team
