# ghar-ka-khana
Modern, responsive React landing page for Ghar Ka Khana with menu filtering, smooth UI, and Tailwind CSS.
# 🏠 Ghar Ka Khana

A modern, aesthetic, and responsive landing page for "Ghar Ka Khana" - an Indian food shop offering homestyle meals.

## ✨ Features

- **Modern Design**: Clean, warm aesthetic with cream and orange color palette
- **Fully Responsive**: Mobile-first approach, works seamlessly on all devices
- **Smooth Animations**: Subtle hover effects and transitions
- **Sticky Navigation**: Always accessible menu bar with smooth scrolling
- **Interactive Menu**: Category-based filtering for easy browsing
- **Featured Items**: Highlight popular dishes
- **Value Combos**: Showcase special deals and savings
- **Contact Form**: Easy way for customers to reach out

## 🛠️ Tech Stack

- **React 18**: Modern React with hooks
- **Tailwind CSS**: Utility-first CSS framework
- **Custom Colors**: Warm cream and orange tones
- **Responsive Design**: Mobile-first approach

## 📁 Project Structure


```
ghar-ka-khana/
├── src/
│   ├── components/
│   │   ├── About.js           # About section
│   │   ├── ComboDeals.js      # Combo deals section
│   │   ├── Contact.js         # Contact section with form
│   │   ├── FeaturedItems.js   # Featured dishes
│   │   ├── Footer.js          # Footer component
│   │   ├── Hero.js            # Hero section with CTA
│   │   ├── MenuSection.js     # Menu with category filtering
│   │   └── Navbar.js          # Sticky navigation
│   ├── data/
│   │   └── menuData.js        # All menu and combo data
│   ├── App.js                 # Main application component
│   ├── index.css              # Tailwind CSS imports
│   └── index.js               # Entry point
├── tailwind.config.js         # Tailwind configuration
├── postcss.config.js          # PostCSS configuration
└── package.json               # Dependencies

```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Navigate to the project directory:**
   ```bash
   cd ghar-ka-khana
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm start
   ```

4. **Open your browser:**
   Navigate to `http://localhost:3000`

### Building for Production

```bash
npm run build
```

## 📝 Menu Categories

The landing page features 6 main menu categories:

1. **Breakfast** ☕ - Coffee, parathas, kebabs, and breakfast items
2. **Main Course** 🍛 - Dal, sabji, paneer dishes
3. **Rice** 🍚 - Pulao, biryani, and rice dishes
4. **Veg Chinese** 🍜 - Noodles, fried rice, manchurian
5. **Combos** 🎁 - Value meal combinations
6. **Frankies** 🌯 - Rolled wraps with various fillings

## 🎨 Design Features

### Color Palette
- **Primary**: Orange (#F97316)
- **Secondary**: Amber (#F59E0B)
- **Background**: Cream (#FFFBF0)
- **Text**: Gray scale for readability

### Typography
- **Headings**: Poppins (clean, modern)
- **Body**: Inter (highly readable)

### Interactive Elements
- Hover effects on cards
- Smooth scroll navigation
- Mobile responsive menu
- Category filtering
- Form validation

## 📱 Responsive Breakpoints

- **Mobile**: < 640px
- **Tablet**: 640px - 1024px
- **Desktop**: > 1024px

## 🎯 Key Sections

1. **Hero Section**: Eye-catching header with CTA buttons
2. **About Section**: Company story and values
3. **Menu Section**: Full menu with category filtering
4. **Featured Items**: Popular dishes showcase
5. **Combo Deals**: Value propositions and savings
6. **Contact Section**: Contact info and message form
7. **Footer**: Quick links and social media

## 🔧 Customization

### Updating Menu Items

Edit `src/data/menuData.js` to add, remove, or modify menu items:

```javascript
export const menuData = {
  breakfast: {
    name: "Breakfast",
    icon: "☕",
    color: "from-orange-500 to-amber-500",
    items: [
      { name: "Your Item", price: 100 },
      // Add more items
    ]
  },
  // Add more categories
};
```

### Changing Colors

Modify `tailwind.config.js` to customize the color palette:

```javascript
colors: {
  'cream': {
    50: '#FFFBF0',
    // Customize cream shades
  },
  // Add or modify other colors
}
```

### Updating Contact Information

Edit `src/components/Contact.js` and `src/components/Footer.js` to update:
- Phone numbers
- Address
- Email
- Working hours

## 🌐 Deployment

### Vercel
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm run build
# Deploy the 'build' folder
```

### GitHub Pages
```bash
npm run build
# Push to GitHub and enable GitHub Pages
```

## 📄 License

This project is open source and available for personal and commercial use.

## 👨‍💻 Support

For questions or support, please reach out through the contact form on the website or email at orders@gharkakhana.com

---

**Made with ❤️ by Ghar Ka Khana Team**
