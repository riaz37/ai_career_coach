# Sensai - AI Career Coach 🚀

Sensai is a full-stack AI-powered career development platform built with modern web technologies. It helps users create professional resumes, prepare for interviews, and track their career progress with AI-driven insights.

![Sensai Platform](https://github.com/user-attachments/assets/eee79242-4056-4d19-b655-2873788979e1)

## 🌟 Features

- **AI-Powered Resume Builder**
  - ATS-optimized resume generation
  - Real-time markdown preview
  - PDF export functionality
  - Auto-save feature

- **Smart Interview Preparation**
  - Industry-specific practice questions
  - AI-driven feedback
  - Performance analytics

- **Career Progress Tracking**
  - Detailed analytics dashboard
  - Skill development insights
  - Industry trend analysis

## 🛠️ Tech Stack

- **Frontend**
  - Next.js 14 (App Router)
  - Tailwind CSS
  - Shadcn UI
  - React Hook Form
  - Zod Validation

- **Backend**
  - Neon DB (PostgreSQL)
  - Prisma ORM
  - Inngest (Background Jobs)
  - Clerk (Authentication)

- **AI Integration**
  - Google Gemini AI
  - Custom AI Prompts

## 📋 Prerequisites

- Node.js 18.17.0 or higher
- PNPM package manager
- PostgreSQL database
- Google Cloud account (for Gemini AI)
- Clerk account

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/sensai-career-coach.git
   cd sensai-career-coach
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory with the following variables:
   ```env
   DATABASE_URL=
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
   CLERK_SECRET_KEY=
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding
   GEMINI_API_KEY=
   ```

4. **Initialize the database**
   ```bash
   pnpm prisma generate
   pnpm prisma db push
   ```

5. **Run the development server**
   ```bash
   pnpm dev
   ```

## 📦 Project Structure

```
sensai/
├── app/                  # Next.js app router
│   ├── (auth)/          # Authentication routes
│   ├── (main)/          # Main application routes
│   └── api/             # API routes
├── components/          # Reusable components
├── lib/                 # Utility functions
├── prisma/             # Database schema
├── public/             # Static assets
└── styles/             # Global styles
```

## 🔒 Authentication Flow

1. User signs up/logs in using Clerk
2. Redirected to onboarding if first-time user
3. Session management handled by Clerk
4. Protected routes using Clerk middleware

## 💾 Database Schema

Key models include:
- User
- Resume
- Interview
- Progress
- Analytics

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com)
- [Shadcn UI](https://ui.shadcn.com)
- [Clerk](https://clerk.dev)
- [Neon Database](https://neon.tech)
- [Google Gemini AI](https://ai.google.dev)

## 📞 Support

For support, email riaz37.ipe@gmail.com or join our Discord community.

---
Built with 💗 by Riaz
