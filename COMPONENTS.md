# 🧩 Component Overview

This document provides a detailed overview of all components in the Ghar Ka Khana landing page.

## 📁 Component Structure

```
src/
├── App.js                 # Main application component
├── index.js              # Entry point
├── index.css             # Global styles
└── components/
    ├── Navbar.js         # Navigation bar
    ├── Hero.js           # Hero section
    ├── About.js          # About section
    ├── MenuSection.js    # Menu with categories
    ├── FeaturedItems.js  # Featured dishes
    ├── ComboDeals.js     # Combo deals
    ├── Contact.js        # Contact section
    └── Footer.js         # Footer
```

## 🎯 Component Details

### 1. **App.js** - Main Application
**Purpose**: Root component that manages scroll tracking and renders all sections.

**Key Features**:
- Scroll position tracking for active navigation
- Smooth scrolling integration
- Component composition

**Props**: None (internal state management)

**State**:
- `activeSection`: Current visible section based on scroll

---

### 2. **Navbar.js** - Sticky Navigation
**Purpose**: Provides navigation to all sections with smooth scrolling.

**Key Features**:
- Sticky positioning with background blur on scroll
- Active section highlighting
- Mobile-responsive hamburger menu
- Smooth scroll to sections

**Props**:
- `activeSection`: Currently visible section ID

**Responsive Behavior**:
- Desktop: Horizontal menu links + CTA button
- Mobile: Hamburger menu with vertical links

---

### 3. **Hero.js** - Hero Section
**Purpose**: Eye-catching header section with branding and CTAs.

**Key Features**:
- Animated background gradients
- Floating food emojis
- Dual CTA buttons (View Menu, Combos)
- Statistics display
- Scroll indicator

**Sections**:
- Main heading with brand name
- Tagline and description
- Feature badges (Fresh Daily, Affordable, Made with Love)
- CTA buttons
- Stats (Menu Items, Categories, Starting Price, Rating)
- Scroll indicator

---

### 4. **About.js** - About Section
**Purpose**: Company story and value proposition.

**Key Features**:
- Feature cards with icons
- Company statistics
- Why Choose Us grid
- Responsive layout

**Content**:
- Brand story and mission
- 4 feature cards (Homemade Taste, Pocket Friendly, Fresh Ingredients, Quick Service)
- Why Choose Us section with 4 benefits
- Badges (Since 2020, 100% Vegetarian)

---

### 5. **MenuSection.js** - Menu Display
**Purpose**: Display all menu items with category filtering.

**Key Features**:
- Category tab filtering
- Price-based statistics
- Add to cart buttons
- Responsive grid layout

**Categories**:
- Breakfast (24 items)
- Main Course (20 items)
- Rice (7 items)
- Veg Chinese (6 items)
- Combos (8 items)
- Frankies (6 items)

**Interactive Elements**:
- Category tab switching
- Hover effects on menu cards
- Price statistics (min, max, average)

---

### 6. **FeaturedItems.js** - Featured Dishes
**Purpose**: Showcase popular and best-selling items.

**Key Features**:
- Large card layout with emoji icons
- Popular badge
- Add to cart functionality
- Hover animations

**Featured Items**:
- Paneer Butter Masala (₹180)
- Veg Biryani (₹180)
- Chole Bhature (₹70)
- Paneer Frankie (₹110)

**Additional Content**:
- Why These Are Best Sellers section
- 4 benefit cards (Top Rated, Most Ordered, Family Favorite, Premium Quality)

---

### 7. **ComboDeals.js** - Value Combos
**Purpose**: Display combo meal deals with savings.

**Key Features**:
- Original vs discounted price display
- Savings calculation
- Popular badge for top deals
- Detailed item lists

**Combo Deals**:
- Budget Thali (₹60, save ₹20)
- Student Special (₹80, save ₹20)
- Punjabi Feast (₹120, save ₹30) - Popular
- Combo Lunch (₹80, save ₹20)

**Sections**:
- Combo cards with details
- Why Order Combos section
- Call-to-action banner

---

### 8. **Contact.js** - Contact Section
**Purpose**: Provide contact information and message form.

**Key Features**:
- Contact information display
- Responsive contact form
- Quick action buttons (WhatsApp, Call)
- Form validation

**Contact Information**:
- Address with emoji icons
- Phone numbers
- Email address
- Working hours

**Form Fields**:
- Name (required)
- Phone number (required)
- Message (required)

---

### 9. **Footer.js** - Footer Component
**Purpose**: Site navigation, links, and branding.

**Key Features**:
- Brand section with social links
- Quick links navigation
- Contact information
- Copyright and legal links

**Sections**:
- Brand (logo, description, social media)
- Quick Links (6 navigation links)
- Contact Info (address, phone, email, hours)
- Bottom bar (copyright, legal links)

---

## 🎨 Styling Conventions

### Color Usage
- **Primary Actions**: Orange-500 (#F97316)
- **Secondary Actions**: Amber-500 (#F59E0B)
- **Backgrounds**: Cream-50 (#FFFBF0), White
- **Text**: Gray-900 (headings), Gray-600 (body), Gray-400 (subtle)

### Spacing
- Section padding: py-20 (80px)
- Card padding: p-6 (24px)
- Gap between elements: gap-4 to gap-12

### Typography
- Headings: text-2xl to text-5xl, font-bold
- Body: text-base to text-lg
- Small text: text-sm

---

## 🔧 Component Props Reference

### Props Flow

```
App.js
├── Navbar.js
│   └── activeSection: string
├── Hero.js (no props)
├── About.js (no props)
├── MenuSection.js (no props)
├── FeaturedItems.js (no props)
├── ComboDeals.js (no props)
├── Contact.js (no props)
└── Footer.js (no props)
```

---

## 🚀 Component Reusability

All components are designed to be:
- **Independent**: Each component can work alone
- **Configurable**: Easy to modify content and styling
- **Responsive**: Work on all screen sizes
- **Accessible**: Proper semantic HTML and ARIA attributes

---

## 📝 Adding New Components

To add a new section:

1. Create component file in `src/components/`
2. Import and add to `App.js`
3. Add navigation link in `Navbar.js`
4. Add quick link in `Footer.js`
5. Update documentation

Example:
```javascript
// NewSection.js
const NewSection = () => {
  return (
    <section id="new-section">
      {/* Content */}
    </section>
  );
};
export default NewSection;
```

---

## 🎯 Best Practices

- Use semantic HTML elements
- Implement proper hover states
- Ensure mobile responsiveness
- Add loading states where needed
- Keep components focused and single-purpose
- Use Tailwind utilities for styling
- Implement proper error handling

---

**Happy Component Building! 🎉**