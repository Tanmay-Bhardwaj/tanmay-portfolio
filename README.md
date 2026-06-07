# 🌟 Tanmay Portfolio - Premium Digital Experience

> A production-ready, database-backed personal portfolio platform with CMS, Journey Forest, Documentary Mode, and AI Clone.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Tanmay-Bhardwaj/tanmay-portfolio)

## ✨ Features

### Core Sections
- 🎭 **Cinematic Hero** - Premium introduction with documentary-style storytelling
- 👤 **About Me** - Elegant personal narrative
- 🎯 **Activities** - Clubs, communities, speaking engagements
- 💼 **Skills** - Refined skill showcase with proficiency indicators
- 🎓 **Certifications** - Polished credential gallery
- 🚀 **Projects** - Editorial-style project presentations
- 🌳 **Journey Forest** - Interactive 3D life map (React Three Fiber)
- 🔬 **Research** - Knowledge archive and technical findings
- 📝 **Blog** - Full-featured blog with categories
- 💬 **Testimonials** - Trust-building social proof
- 🖼️ **Gallery** - Elegant photo masonry
- 🤖 **AI Clone** - "Ask Future Tanmay" with RAG
- 📞 **Contact** - Professional contact form

### Admin Features
- 🔐 **Secure Admin Panel** (`/admin`) - Protected with NextAuth
- ✏️ **Full CRUD Operations** - Manage all content types
- 📸 **Image Upload System** - Cloudinary integration
- 📊 **Dashboard Overview** - Content statistics
- 🔄 **Publish/Unpublish** - Content visibility control

### Experience Features
- 🎬 **Documentary Mode** - Scroll-based cinematic storytelling
- 🗺️ **Interactive Life Map** - Zoomable universe-style navigation
- 🌲 **Journey Forest** - Living 3D world of milestones
- 🤖 **AI Knowledge Assistant** - Context-aware Q&A

### Technical Excellence
- ⚡ **Optimized for Vercel** - Fast deployment, edge functions
- 🗄️ **PostgreSQL + Prisma** - Type-safe database operations
- 🔒 **NextAuth** - Secure authentication
- 🎨 **JP Morgan-Inspired Design** - Premium, elegant aesthetic
- 📱 **Fully Responsive** - Mobile, tablet, desktop optimized
- ♿ **Accessible** - WCAG compliant
- 🔍 **SEO Ready** - Metadata, Open Graph, sitemaps

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- PostgreSQL database (local or cloud)
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/Tanmay-Bhardwaj/tanmay-portfolio.git
cd tanmay-portfolio

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your credentials

# Initialize database
npx prisma generate
npx prisma db push
npx prisma db seed

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see your portfolio.

---

## 🗄️ Database Schema

The platform uses **Prisma ORM** with PostgreSQL:

- **User** - Admin authentication
- **About** - Personal information
- **Activity** - Clubs, communities, events
- **Skill** - Technical and soft skills
- **Certification** - Credentials and awards
- **Project** - Portfolio work
- **Research** - Technical explorations
- **BlogPost** - Articles and writings
- **Testimonial** - Social proof
- **GalleryItem** - Photos and media
- **JourneyNode** - Forest milestones
- **Contact** - Form submissions

---

## 🎨 Design System

### Color Palette (JP Morgan Inspired)
```typescript
const colors = {
  navy: '#0A1929',      // Deep Navy
  slate: '#2E3944',     // Rich Slate
  ivory: '#F5F0E6',     // Warm Ivory
  gold: '#C8A951',      // Antique Gold
  emerald: '#2D5016',   // Soft Emerald
  bronze: '#8B6F47',    // Muted Bronze
  champagne: '#F4E8D0'  // Champagne
}
```

### Typography
- **Headings**: Playfair Display (serif elegance)
- **Body**: Inter (modern readability)
- **Accent**: Dancing Script (cursive signatures)

---

## 🔧 Environment Variables

```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/tanmay_portfolio"

# NextAuth
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="generate-with-openssl-rand-base64-32"

# Admin Credentials
ADMIN_EMAIL="your-email@example.com"
ADMIN_PASSWORD="secure-password"

# Cloudinary (optional)
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME="your-cloud-name"
CLOUDINARY_API_KEY="your-api-key"
CLOUDINARY_API_SECRET="your-api-secret"

# OpenAI (for AI Clone)
OPENAI_API_KEY="sk-..."
```

---

## 📁 Project Structure

```
tanmay-portfolio/
├── app/
│   ├── (main)/              # Public pages
│   │   ├── page.tsx         # Hero + all sections
│   │   ├── blog/            # Blog system
│   │   ├── projects/        # Project detail pages
│   │   └── layout.tsx       # Main layout
│   ├── admin/               # Admin panel
│   │   ├── dashboard/
│   │   ├── content/
│   │   └── layout.tsx
│   ├── api/                 # API routes
│   │   ├── auth/            # NextAuth
│   │   ├── content/         # CRUD endpoints
│   │   └── ai-clone/        # AI Q&A
│   └── globals.css
├── components/
│   ├── sections/            # Main page sections
│   ├── admin/               # Admin components
│   ├── forest/              # Journey Forest 3D
│   ├── documentary/         # Documentary mode
│   └── ui/                  # Design system
├── lib/
│   ├── prisma.ts
│   ├── auth.ts
│   └── utils.ts
├── prisma/
│   ├── schema.prisma
│   └── seed.ts
├── public/
│   └── images/
└── package.json
```

---

## 🔐 Admin Panel

Access the admin panel at: **`/admin`**

### Default Credentials (after seeding)
- Email: Set in `.env.local`
- Password: Set in `.env.local`

### Admin Features
1. **Dashboard** - Overview statistics
2. **Content Management**
   - About Me
   - Activities
   - Skills
   - Certifications
   - Projects
   - Research
   - Blog Posts
   - Testimonials
   - Gallery
   - Journey Nodes
3. **Media Library** - Upload and manage images
4. **Settings** - Site configuration

---

## 🌳 Journey Forest

The Journey Forest is a **3D interactive experience** built with:
- **React Three Fiber** - React renderer for Three.js
- **@react-three/drei** - Helpers and abstractions
- **Framer Motion 3D** - Smooth animations

### Features
- Zoomable exploration (5 levels)
- Clickable tree milestones
- Atmospheric particles
- Dynamic lighting
- Performance optimized (60 FPS)

---

## 🎬 Documentary Mode

Toggle documentary mode with **"Watch My Story"** button:
- Scroll-based scene transitions
- Photo reveals with parallax
- Milestone animations
- Chapter progress indicator
- Elegant narration blocks

---

## 🤖 AI Clone

The AI Clone uses **OpenAI GPT-4o-mini** with RAG:
1. Retrieves relevant content from database
2. Builds context from projects, blog, skills
3. Generates personalized responses
4. Falls back to seed answers without API key

---

## 🚀 Deployment

### Deploy to Vercel

1. **Push to GitHub**
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. **Import to Vercel**
   - Go to [vercel.com/new](https://vercel.com/new)
   - Import your repository
   - Add environment variables
   - Deploy

3. **Set up Database**
   - Use Vercel Postgres or external PostgreSQL
   - Update `DATABASE_URL` in Vercel environment
   - Run migrations: `npx prisma migrate deploy`

### Post-Deployment
1. Run database seed: `npx prisma db seed`
2. Test admin login at `yourdomain.com/admin`
3. Customize content via admin panel
4. Upload your images

---

## 📝 Content Management

### Adding Content
1. Log in to `/admin`
2. Navigate to desired content type
3. Click "Add New"
4. Fill in the form
5. Upload images if needed
6. Click "Publish"

### Journey Forest Nodes
Each node represents a life milestone:
- **Title** - Event name
- **Date** - When it happened
- **Type** - sapling, medium, ancient
- **Description** - Story behind it
- **Position** - 3D coordinates (auto-calculated)
- **Impact/Growth Scores** - Visual sizing

---

## 🎨 Customization

### Colors
Edit `app/globals.css` CSS variables:

```css
:root {
  --navy: #0A1929;
  --gold: #C8A951;
  /* ... */
}
```

### Typography
Update `tailwind.config.ts`:

```typescript
fontFamily: {
  display: ['Playfair Display', 'serif'],
  sans: ['Inter', 'sans-serif'],
  cursive: ['Dancing Script', 'cursive'],
}
```

---

## 🐛 Troubleshooting

### Database Connection Issues
```bash
# Regenerate Prisma Client
npx prisma generate

# Push schema changes
npx prisma db push
```

### Admin Login Fails
- Check `NEXTAUTH_SECRET` is set
- Verify admin credentials in database
- Clear browser cookies

### Journey Forest Not Loading
- Ensure WebGL is supported
- Check browser console for errors
- Try reducing particle count in config

---

## 📚 Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Database**: PostgreSQL + Prisma ORM
- **Auth**: NextAuth.js
- **Styling**: Tailwind CSS
- **3D**: React Three Fiber + Three.js
- **Animation**: Framer Motion
- **Forms**: React Hook Form
- **Validation**: Zod
- **Image Upload**: Cloudinary
- **AI**: OpenAI API
- **Deployment**: Vercel

---

## 📖 Documentation

- [Next.js Docs](https://nextjs.org/docs)
- [Prisma Docs](https://www.prisma.io/docs)
- [NextAuth Docs](https://next-auth.js.org)
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber)
- [Tailwind CSS](https://tailwindcss.com/docs)

---

## 🤝 Contributing

This is a personal portfolio template. Feel free to fork and customize for your own use.

---

## 📄 License

MIT License - feel free to use this template for your own portfolio.

---

## 🙏 Acknowledgments

- Design inspiration: JP Morgan, luxury financial brands
- 3D forest concept: Interactive life mapping
- Documentary mode: Premium editorial experiences

---

**Built with ❤️ for storytelling and premium digital experiences.**
