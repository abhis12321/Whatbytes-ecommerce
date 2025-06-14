# WhatBytes E-commerce Store

A modern, responsive e-commerce application built with Next.js 15, React 18, and Tailwind CSS. Features a complete shopping experience with product browsing, filtering, search, and cart management.

🚀 **Live Demo**: [https://whatbytes-ecommerce.vercel.app/](https://whatbytes-ecommerce.vercel.app/)

## ✨ Features

### 🏠 Home Page
- **Responsive Product Grid**: 3 columns on desktop, 2 on tablet, 1 on mobile
- **Advanced Filtering**: Category, price range, and brand filters
- **Real-time Search**: Instant product search with string matching
- **URL-based Filters**: Shareable URLs with filter parameters
- **Sticky Header**: Logo, search bar, cart badge, and profile icon

### 🛍️ Product Details
- **Dynamic Routing**: SEO-friendly URLs (`/product/[id]`)
- **Product Gallery**: High-quality product images
- **Detailed Information**: Title, price, description, ratings, and reviews
- **Quantity Selector**: Add multiple items to cart
- **Related Products**: Smart product recommendations

### 🛒 Shopping Cart
- **Persistent Storage**: Cart state saved in localStorage
- **Quantity Management**: Update quantities or remove items
- **Price Calculation**: Real-time total and subtotal calculations
- **Empty State**: Helpful messaging when cart is empty

### 📱 Responsive Design
- **Mobile-First**: Optimized for all screen sizes
- **Touch-Friendly**: Large tap targets and smooth interactions
- **Accessible**: ARIA labels and keyboard navigation support

## 🛠️ Tech Stack

- **Framework**: Next.js 15 (App Router)
- **Frontend**: React 18 with JSX
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **State Management**: React Context + useReducer
- **Routing**: Next.js App Router with dynamic routes
- **Image Optimization**: Next.js Image component
- **Deployment**: Vercel

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone the repository**
   \`\`\`bash
   git clone https://github.com/yourusername/whatbytes-ecommerce.git
   cd whatbytes-ecommerce
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   # or
   yarn install
   \`\`\`

3. **Run the development server**
   \`\`\`bash
   npm run dev
   # or
   yarn dev
   \`\`\`

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📁 Project Structure

\`\`\`
whatbytes-ecommerce/
├── app/
│   ├── components/          # Reusable React components
│   │   ├── Header.jsx       # Navigation header
│   │   ├── Sidebar.jsx      # Filter sidebar
│   │   ├── ProductCard.jsx  # Product display card
│   │   ├── ProductGrid.jsx  # Product grid layout
│   │   └── Footer.jsx       # Site footer
│   ├── context/             # React Context providers
│   │   └── CartContext.jsx  # Shopping cart state management
│   ├── data/                # Static data and mock APIs
│   │   └── products.js      # Product catalog data
│   ├── product/[id]/        # Dynamic product pages
│   │   └── page.jsx         # Product detail page
│   ├── cart/                # Shopping cart page
│   │   └── page.jsx         # Cart management page
│   ├── globals.css          # Global styles and Tailwind imports
│   ├── layout.jsx           # Root layout component
│   ├── loading.jsx          # Loading UI component
│   └── page.jsx             # Home page component
├── public/                  # Static assets
├── next.config.js           # Next.js configuration
├── tailwind.config.js       # Tailwind CSS configuration
├── postcss.config.js        # PostCSS configuration
└── package.json             # Dependencies and scripts
\`\`\`

## 🎯 Key Features Implementation

### State Management
- **React Context**: Global cart state management
- **useReducer**: Complex state logic for cart operations
- **localStorage**: Persistent cart data across sessions

### Filtering System
- **Category Filters**: Checkbox-based category selection
- **Price Range**: Interactive slider for price filtering
- **Brand Filters**: Multi-select brand filtering
- **Search**: Real-time text-based product search

### URL Management
- **Query Parameters**: Filter state reflected in URL
- **Shareable Links**: Users can share filtered product views
- **Browser History**: Proper back/forward navigation

### Performance Optimizations
- **Image Optimization**: Next.js Image component with proper sizing
- **Code Splitting**: Automatic route-based code splitting
- **Memoization**: React.memo and useMemo for expensive operations
- **Lazy Loading**: Images loaded on demand

## 🔧 Configuration

### Environment Variables
Create a \`.env.local\` file for environment-specific configurations:

\`\`\`env
NEXT_PUBLIC_SITE_URL=https://yoursite.com
\`\`\`

### Tailwind Configuration
The project uses a custom Tailwind configuration with:
- Custom color palette
- Responsive breakpoints
- Component utilities
- CSS custom properties support

## 📱 Responsive Breakpoints

- **Mobile**: < 640px (1 column grid)
- **Tablet**: 640px - 1024px (2 column grid)  
- **Desktop**: > 1024px (3 column grid)
- **Large Desktop**: > 1280px (optimized spacing)

## 🧪 Testing

\`\`\`bash
# Run linting
npm run lint

# Build for production
npm run build

# Start production server
npm run start
\`\`\`

## 🚀 Deployment

### Vercel (Recommended)

1. **Connect to Vercel**
   - Push your code to GitHub
   - Connect your repository to Vercel
   - Deploy automatically on push

2. **Manual Deployment**
   \`\`\`bash
   npm run build
   vercel --prod
   \`\`\`

### Other Platforms
The app can be deployed to any platform that supports Next.js:
- Netlify
- AWS Amplify
- Railway
- DigitalOcean App Platform

## 🎨 Customization

### Adding New Products
Edit \`app/data/products.js\` to add new products:

\`\`\`javascript
{
  id: 16,
  title: "New Product",
  price: 99.99,
  category: "electronics",
  brand: "BrandName",
  image: "https://example.com/image.jpg",
  description: "Product description",
  rating: 4.5,
  reviews: 100,
}
\`\`\`

### Styling Changes
- Modify \`tailwind.config.js\` for theme customization
- Update \`app/globals.css\` for global styles
- Component-specific styles in individual JSX files

### Adding New Features
- Create new components in \`app/components/\`
- Add new pages in appropriate directories
- Extend context providers for additional state

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (\`git checkout -b feature/amazing-feature\`)
3. Commit your changes (\`git commit -m 'Add amazing feature'\`)
4. Push to the branch (\`git push origin feature/amazing-feature\`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Next.js Team** - For the amazing React framework
- **Tailwind CSS** - For the utility-first CSS framework
- **Lucide** - For the beautiful icon library
- **Unsplash** - For high-quality product images

## 📞 Support

If you have any questions or need help with setup, please:
- Open an issue on GitHub
- Check the [Next.js documentation](https://nextjs.org/docs)
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)

---

**Built with ❤️ using Next.js 15 and React 18**
