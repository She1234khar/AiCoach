# 🚀 AspireAI – AI-Powered Career Development Platform  



AspireAI is an advanced, AI-powered career development platform designed to guide users through every step of their professional journey.  
Whether you're crafting the perfect resume, preparing for interviews, or navigating industry shifts, AspireAI provides intelligent, real-time support to supercharge your career.  

---

## ✨ Features  

- 🤖 AI-Powered Career Guidance – Personalized career path suggestions & role-specific advice.  
- 📄 Smart Resume Creation– ATS-optimized resumes with keyword suggestions.  
- 🎤 Interview Preparation – Role-based practice with real-time AI feedback.  
- 📊 Industry Insights – Salary trends, in-demand roles, and skill insights.  
- 📝 Cover Letter Generation – Tailored letters for specific job listings.  
- 📈 Continuous Career Development – Learning paths, skill assessments, and course recommendations.  
- 💎 AI Token System – Credit-based usage powered by **Razorpay** (earn via subscription or direct purchase).  

🔗 **Live Demo:** [Click Here](ai-career-sense.vercel.app)  

## 🛠 Tech Stack  

Frontend: Next.js 15, React 19, TailwindCSS  
Backend: Next.js API Routes, Prisma ORM  
Database: PostgreSQL  
Authentication: Clerk.dev  
AI Integration: Google Generative AI (PaLM)  
UI Library: Radix UI, Lucide Icons  
Payments: Razorpay  
Deployment: Vercel  

---

## ⚡ Getting Started  

### 🔧 Prerequisites  
- Node.js v18+  
- PostgreSQL installed & running  
- Clerk account (for auth)  
- Google AI API Key  
- Razorpay account  

### 📁 Environment Setup  

Create a .env file in the root directory:  

env
# PostgreSQL Database
DATABASE_URL="postgresql://username:password@localhost:5432/aspireai"

# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

# Google Generative AI
GOOGLE_AI_API_KEY=your_google_ai_api_key

# Razorpay
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret

📦 Installation

# Clone repository
git clone https://github.com/she1234khar/aspireai.git
cd aspireai

# Install dependencies
npm install

# Database setup
npx prisma migrate dev
npx prisma db seed

# Start development server
npm run dev

Visit 👉 http://localhost:3000

## 📂 Project Structure  

```bash
aspireai/
├── app/                  # Next.js app directory
│   ├── (main)/           # Main application routes
│   ├── api/              # API routes (auth, AI, payments)
│   └── lib/              # Utility functions
├── components/           # Reusable React UI components
├── actions/              # Server actions / data operations
├── data/                 # Static data & constants
├── prisma/               # Prisma schema & migrations
│   ├── schema.prisma     
│   └── seed.js           
├── public/               # Static files
└── .env                  # Environment variables

