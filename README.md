FirstlightMail

A modern, fast, and minimal email management web app built with Next.js and Supabase.

Features

User Authentication – Sign up and log in securely with OAuth or email/password.

Email Management – View and organize your emails in a clean interface.

Minimal Design – Simple black-and-white aesthetic for distraction-free email handling.

Responsive – Works seamlessly on desktops, tablets, and mobile devices.

Fast Performance – Built with modern Next.js architecture.

Tech Stack

Framework: Next.js 14 with App Router

Authentication & Backend: Supabase

UI Components: shadcn/ui

Styling: Tailwind CSS

Language: TypeScript

Getting Started
Prerequisites

Node.js 18+

npm or yarn

Supabase account (or any preferred backend)

Installation

Clone the repository:

git clone <your-repo-url>
cd firstlightmail


Install dependencies:

npm install


Configure environment variables:
Create a .env.local file with your Supabase or backend credentials:

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key


Run the development server:

npm run dev


Open your browser at http://localhost:3000

Project Structure
src/
├── app/                # Next.js App Router
│   ├── dashboard/      # Dashboard page
│   ├── login/          # Login page
│   ├── signup/         # Signup page
│   └── layout.tsx      # Root layout
├── components/         # UI components
│   └── ui/             # shadcn/ui components
├── contexts/           # React contexts
│   └── AuthContext.tsx # Authentication context
└── lib/                # Utility functions
    ├── supabase.ts     # Supabase client
    └── utils.ts        # General utilities

Pages

Landing Page (/) – Hero section, features overview, and call-to-action buttons.

Login Page (/login) – Sign in with OAuth or email/password.

Signup Page (/signup) – Create an account easily.

Dashboard (/dashboard) – View profile info and manage emails.

Deployment

The project can be deployed to any platform that supports Next.js:

Vercel – Recommended for easy setup.

Other Platforms – Netlify, Railway, DigitalOcean App Platform, etc.

Contributing

Fork the repository

Create a new branch

Make your changes

Submit a pull request

License

MIT License

Support

For support, create an issue in the repository.
