# FirstlightAI

A modern, AI-powered email assistant built with Next.js, Supabase, and shadcn/ui.

## Features

- 🔐 **Google OAuth Integration** - Seamless authentication with Google
- 📧 **Email Management** - View and organize your emails
- 🎨 **Minimal Design** - Clean black and white aesthetic
- ⚡ **Fast Performance** - Built with Next.js 14 and App Router
- 📱 **Responsive** - Works perfectly on all devices

## Tech Stack

- **Framework**: Next.js 14 with App Router
- **Authentication**: Supabase Auth with Google OAuth
- **UI Components**: shadcn/ui
- **Styling**: Tailwind CSS
- **Language**: TypeScript

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- Supabase account

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd firstlight-ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up Supabase**
   - Create a new project at [supabase.com](https://supabase.com)
   - Go to Settings > API to get your project URL and anon key
   - Enable Google OAuth in Authentication > Providers

4. **Environment Variables**
   Create a `.env.local` file in the root directory:
   ```env
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
   ```

5. **Run the development server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## Project Structure

```
src/
├── app/                    # Next.js App Router
│   ├── dashboard/         # Dashboard page
│   ├── login/            # Login page
│   ├── signup/           # Signup page
│   └── layout.tsx        # Root layout
├── components/            # UI components
│   └── ui/               # shadcn/ui components
├── contexts/             # React contexts
│   └── AuthContext.tsx   # Authentication context
└── lib/                  # Utility functions
    ├── supabase.ts       # Supabase client
    └── utils.ts          # General utilities
```

## Pages

### Landing Page (`/`)
- Beautiful hero section
- Feature highlights
- Call-to-action buttons

### Login Page (`/login`)
- Google OAuth integration
- Email/password login
- Clean, minimal design

### Signup Page (`/signup`)
- Google OAuth signup
- Email registration
- Password confirmation

### Dashboard (`/dashboard`)
- User profile information
- Recent emails display
- Account management

## Authentication Flow

1. **Google OAuth**: Users can sign in/up with their Google account
2. **Email/Password**: Traditional email and password authentication
3. **Session Management**: Automatic session handling with Supabase
4. **Protected Routes**: Dashboard requires authentication

## Styling

The project uses a minimal black and white design with:
- **Primary**: Black (`#000000`)
- **Secondary**: White (`#ffffff`)
- **Accents**: Gray tones for subtle variations
- **Typography**: Inter font family
- **Components**: shadcn/ui for consistent design

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy automatically

### Other Platforms

The project can be deployed to any platform that supports Next.js:
- Netlify
- Railway
- DigitalOcean App Platform

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `NEXT_PUBLIC_SUPABASE_URL` | Your Supabase project URL | Yes |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Your Supabase anon key | Yes |
| `SUPABASE_SERVICE_ROLE_KEY` | Your Supabase service role key | Yes |

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For support, email support@firstlight.ai or create an issue in the repository.
