# Design Guidelines: Artistic Portfolio Website

## Design Approach
**Reference-Based**: Draw inspiration from artistic portfolio websites and creative agency sites (Squarespace templates, Cargo Collective, Behance portfolios) with a warm, handcrafted aesthetic. The design emphasizes organic shapes, decorative elements, and a gallery-like presentation.

## Color Palette (From Screenshots)
- **Primary Background**: Warm beige/cream (#F5EFE7, #F8F3ED)
- **Accent Background**: Soft peach/terracotta tones
- **Text**: Dark charcoal/black for high contrast readability
- **Borders/Decorative**: Brown/burnt sienna for frames and patterns
- **Card Backgrounds**: White/off-white for polaroid-style cards

## Typography Hierarchy
- **Headers (H1)**: 48-64px (mobile: 32-40px), bold serif or artistic display font
- **Section Titles (H2)**: 36-48px (mobile: 28-32px), medium weight
- **Service Cards**: 24-28px titles, 16-18px body text
- **Body Text**: 16-18px, comfortable line-height (1.6-1.8)
- **Navigation**: 16px, medium weight, uppercase or small caps

## Layout System
**Spacing Units**: Use Tailwind units of 4, 6, 8, 12, 16, 20 for consistent rhythm
- Section padding: `py-16 md:py-20 lg:py-24`
- Container max-width: `max-w-7xl mx-auto px-6 md:px-8`
- Card spacing: `gap-8 md:gap-12`

## Component Library

### Navigation
- Horizontal menu with smooth background on scroll
- Logo on left, menu items right-aligned
- Mobile: Hamburger menu with slide-in drawer
- Links: Homepage, Contact, Portfolio, Services, About Us

### Hero Section
- Full-width with decorative brushstroke/organic shape overlays
- Centered headline with artistic typography
- Subtle texture or pattern background
- CTA button with rounded corners, generous padding

### Services Section (Polaroid Cards)
- 3-column grid (1 column mobile, 2 tablet, 3 desktop)
- White card backgrounds with subtle shadow
- Top-heavy image area with thin border frame
- Service title below image
- Decorative border pattern surrounding the entire section (continuous geometric or floral pattern)
- Cards: Film Production, Branding, Art Curation

### Film Production Detail Section
- Quote/headline at top with decorative quotation marks
- Image showcase grid (2-3 images)
- Bulleted service list with custom markers
- Decorative camera/film illustrations as accent elements
- Asymmetric layout for visual interest

### Contact Form
- Clean, spacious form layout with generous field spacing
- Input fields: Full-width with subtle borders, rounded corners (rounded-lg)
- Placeholder text in muted color
- Fields: Name, Email, Phone, Message (textarea)
- Submit button: Prominent, warm color, rounded-full or rounded-xl
- Success message: Centered overlay or inline message with checkmark icon
- Error states: Red border on invalid fields with helper text below

### Decorative Elements
- Brushstroke accents in section transitions
- Geometric border patterns (squares, diamonds, or traditional motifs)
- Subtle texture overlays on backgrounds
- Hand-drawn style illustrations (camera, art tools)

## Responsive Behavior
- **Mobile (< 768px)**: Single column, stacked navigation, touch-friendly buttons (min-height: 48px)
- **Tablet (768-1024px)**: 2-column grids, adjusted spacing
- **Desktop (> 1024px)**: Full 3-column layouts, expanded whitespace
- Navigation transforms from horizontal to hamburger at md breakpoint

## Images
**Critical Images Needed**:
1. **Hero Background**: Artistic/abstract texture or workspace scene (full-width, subtle)
2. **Service Cards**: 3 polaroid-style images for Film Production, Branding, Art Curation (square format, 600x600px minimum)
3. **Film Production Detail**: 2-3 showcase images of film work (rectangular, various sizes)
4. **Decorative Elements**: Camera illustration, brushstroke graphics (SVG preferred)

No large hero image required - focus on decorative background patterns and service imagery.

## Accessibility & Polish
- Minimum contrast ratio 4.5:1 for body text
- Focus states on all interactive elements with visible outline
- Form labels visible and associated with inputs
- Smooth scroll behavior for internal navigation
- Loading states during form submission
- Consistent hover states: subtle scale or opacity changes

## Animation Guidelines
**Minimal and purposeful**:
- Fade-in on scroll for service cards (intersection observer)
- Smooth transitions on hover (0.2-0.3s duration)
- Form submission: Loading spinner, success checkmark animation
- Navigation: Smooth slide for mobile menu