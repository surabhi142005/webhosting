# Web Hosting Scrollytelling Website

## Concept & Vision
An immersive, colorful scrollytelling experience that takes visitors on a journey through the world of web hosting. As users scroll, they travel through distinct "zones" representing each hosting type, with dynamic animations, vibrant gradients, and engaging visuals that make technical concepts accessible and memorable. The feeling should be futuristic, energetic, and slightly playful—like a tech expo meets a creative portfolio.

## Design Language

### Aesthetic Direction
Cyberpunk-meets-modern-tech with bold gradients, floating elements, glassmorphism cards, and a sense of depth through parallax and layered animations.

### Color Palette
- **Shared Hosting**: `#FF6B6B` (coral red) → `#FFE66D` (warm yellow)
- **VPS Hosting**: `#4ECDC4` (teal) → `#45B7D1` (sky blue)
- **Dedicated Hosting**: `#9B59B6` (royal purple) → `#E74C3C` (crimson)
- **Cloud Hosting**: `#00D9FF` (cyan) → `#667EEA` (indigo)
- **Managed Hosting**: `#F093FB` (pink) → `#F5576C` (rose)
- **Background Dark**: `#0a0a1a`
- **Text Light**: `#ffffff`
- **Text Muted**: `#a0a0c0`

### Typography
- **Headings**: "Space Grotesk" (bold, futuristic)
- **Body**: "Inter" (clean, readable)
- **Accent/Numbers**: "Orbitron" (tech feel)

### Motion Philosophy
- Scroll-triggered reveals with staggered fade-ins
- Parallax depth layers (background elements move slower)
- Floating/pulsing ambient elements
- Smooth section transitions with color palette shifts
- Cards slide in from different directions
- Progress indicator synced to scroll position

## Layout & Structure

### Hero Section
- Full viewport height
- Animated gradient background with floating server icons
- Large headline with typewriter or glitch effect
- Scroll indicator arrow bouncing

### Hosting Type Sections (5 total)
Each section ~100vh with:
- Fixed background gradient (unique per type)
- Floating decorative shapes
- Central content card with glassmorphism
- Icon visualization for the hosting type
- Pros/cons in styled lists
- Scroll-triggered animations

### Comparison Section
- Interactive table with hover effects
- Mobile: swipeable cards
- Color-coded rows matching hosting types

### Footer
- Minimal with gradient line separator
- "Start your journey" CTA

## Features & Interactions

### Scroll Behavior
- Smooth scrolling
- Section snap hints (not enforced)
- Scroll progress bar at top
- Active section indicator

### Micro-interactions
- Cards lift on hover (translateY + shadow)
- Buttons have gradient animation on hover
- Icons pulse subtly
- Links underline animation

### Visual Effects
- Gradient orbs floating in background
- Particle/dot grid pattern
- Subtle noise texture overlay
- Parallax on decorative elements

## Component Inventory

### Hero
- Animated gradient canvas
- Floating server/cloud SVG icons
- Bounce animation scroll indicator

### Hosting Card
- Glassmorphism: `background: rgba(255,255,255,0.1)`, `backdrop-filter: blur(20px)`
- Border: `1px solid rgba(255,255,255,0.2)`
- Icon area, title, description, pros/cons lists
- States: default (in view), hover (lifted)

### Comparison Table
- Sticky header row
- Alternating subtle row backgrounds
- Color dots for hosting types
- Hover: row highlights

### Progress Bar
- Fixed top, full width
- Height: 3px
- Gradient fill matching current section

## Technical Approach
- Single HTML file with embedded CSS and JavaScript
- Vanilla JS for scroll detection and animations
- Intersection Observer API for scroll-triggered reveals
- CSS custom properties for dynamic theming
- CSS animations for ambient motion
- No external frameworks (pure HTML/CSS/JS)
