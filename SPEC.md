# SQL DBA Career Learning Platform - SPEC.md

## 1. Concept & Vision

A sleek, professional educational platform designed to guide aspiring database administrators through the SQL DBA career path. The site feels like stepping into a modern tech company's internal training portal — authoritative yet approachable, with data visualizations that make the career journey tangible and inspiring.

## 2. Design Language

### Aesthetic Direction
Dark mode terminal-inspired aesthetic with vibrant accent colors. References: database management consoles meets modern SaaS dashboard. Clean data visualization aesthetics.

### Color Palette
- **Primary Background**: #0d1117 (deep space black)
- **Secondary Background**: #161b22 (card surfaces)
- **Accent Primary**: #58a6ff (electric blue - links, highlights)
- **Accent Secondary**: #238636 (success green - growth, jobs)
- **Accent Tertiary**: #f78166 (warm orange - warnings, attention)
- **Text Primary**: #c9d1d9 (soft white)
- **Text Secondary**: #8b949e (muted gray)
- **Border**: #30363d

### Typography
- **Headings**: "JetBrains Mono", monospace (technical credibility)
- **Body**: "Inter", sans-serif (readability)
- **Code snippets**: "Fira Code", monospace

### Spatial System
- Base unit: 8px
- Section padding: 80px vertical, 5% horizontal
- Card padding: 24px
- Border radius: 8px (cards), 4px (buttons)

### Motion Philosophy
- Scroll-triggered fade-up animations (opacity 0→1, translateY 20px→0, 500ms ease-out)
- Staggered card reveals (100ms delay between items)
- Hover lift on cards (translateY -4px, box-shadow expansion)
- Progress bar animations on scroll-into-view

### Visual Assets
- Lucide icons throughout
- Custom SVG illustrations for database concepts
- Gradient overlays on hero section
- Animated database/server illustrations

## 3. Layout & Structure

### Page Sections (Single Page Application)
1. **Hero Section** - Full viewport, animated database illustration, compelling headline
2. **What is a SQL DBA** - Role definition with key responsibilities grid
3. **Career Path** - Visual timeline from junior to senior roles
4. **Skills Roadmap** - Interactive skill tree with proficiency levels
5. **Job Market** - Salary ranges, demand statistics, job titles breakdown
6. **Learning Path** - Step-by-step curriculum with resource links
7. **Tools & Technologies** - Technology stack overview with logos
8. **Get Started CTA** - Newsletter signup and next steps

### Responsive Strategy
- Desktop: Multi-column layouts, full animations
- Tablet: 2-column grids collapse to single where needed
- Mobile: Single column, reduced animation, hamburger nav

## 4. Features & Interactions

### Core Features
- **Interactive Skill Cards**: Click to expand with detailed explanations
- **Salary Calculator Visual**: Animated bar charts showing salary ranges
- **Learning Path Timeline**: Vertical timeline with expandable nodes
- **Tool Badges**: Hover reveals tool description popover
- **Smooth Navigation**: Fixed header with scroll-spy active states

### Interaction Details
- Cards lift on hover with shadow expansion
- Skill items show progress bars that animate on scroll
- Timeline nodes pulse on hover
- CTA buttons have gradient shimmer on hover

### States
- Default, hover, active for all interactive elements
- Loading skeleton for any async content
- Empty states with helpful messaging

## 5. Component Inventory

### Navigation Bar
- Fixed top, blur backdrop, logo left, nav links right
- Active link has accent underline
- Mobile: hamburger menu with slide-in drawer

### Hero Section
- Large heading with gradient text
- Subheading with typing animation effect
- CTA buttons (primary/secondary)
- Animated database server illustration

### Info Cards
- Icon + title + description
- Hover lift effect
- Optional badge for "hot skill" or "in-demand"

### Timeline Node
- Circle connector with vertical line
- Role title, company type, salary range
- Expandable details section

### Skill Bar
- Label + percentage bar
- Animated fill on scroll
- Color coded by category

### Tool Badge
- Logo/icon + name
- Hover shows description tooltip

### CTA Section
- Email input + submit button
- Social proof text
- Gradient background

## 6. Technical Approach

- **Framework**: Single HTML file with embedded CSS and vanilla JavaScript
- **No build step required**: Pure frontend, runs directly in browser
- **CSS**: Custom properties for theming, Grid/Flexbox layouts
- **JS**: Intersection Observer for scroll animations, event delegation
- **Fonts**: Google Fonts CDN (JetBrains Mono, Inter, Fira Code)
- **Icons**: Lucide CDN
