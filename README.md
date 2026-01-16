# LiteLists

**The fastest shared list app for households**

LiteLists is a real-time collaborative shopping and packing list app designed for roommates, couples, and small groups. Never forget what to buy or who's getting what – stay synced effortlessly with clean UX and instant updates.

## About

LiteLists helps households and small groups manage shared shopping lists and packing lists with **real-time collaboration** and **automatic cost splitting**. Designed for roommates, couples, and friend groups who want a simple, reliable way to coordinate purchases and tasks.

### What Makes LiteLists Different

- **Clean UX**: Fast, intuitive interface focused on getting things done
- **Reliable Sync**: Real-time updates powered by Supabase – no conflicts, no confusion
- **Simple Cost Splitting**: Add prices per item, auto-calculate split totals
- **Smart Reminders**: Recurring lists and intelligent refill suggestions

## Features (MVP)

- **Spaces**: Create and share households/groups via invite link or QR code
- **Real-time Collaboration**: See live updates with presence indicators showing who's active
- **Item Assignment**: Mark items with "who's on it?" to coordinate shopping
- **Cost Splitting**: Add per-item pricing with automatic split calculations
- **Activity Feed**: Track changes (e.g., "Alice checked off Milk")
- **Recurring Lists**: Set up weekly grocery lists that repeat automatically
- **Smart Reminders**: Get notified when frequently-bought items might need refilling

## Tech Stack

- **Frontend**: 
  - Web: [Next.js](https://nextjs.org/)
  - Mobile: [Expo](https://expo.dev/) (React Native)
- **Backend**: [Supabase](https://supabase.com/) (Auth, Postgres, Realtime, Edge Functions)
- **State Management**: Zustand or Jotai
- **Payments**: Stripe
- **Deployment**: Vercel (web) + EAS (mobile)

## Project Structure

```
/apps
  /web          # Next.js web app
  /mobile       # Expo React Native app
/packages
  /ui           # Shared UI components
  /database     # Supabase schema & migrations
  /shared       # Shared utilities and types
/docs           # Additional documentation
```

## Roadmap

- **Week 1-2**: Core lists + spaces + invites + realtime
- **Week 3**: Splitting + activity feed + presence
- **Week 4**: Recurrence + reminders
- **Week 5**: Polish + onboarding + metrics
- **Week 6**: Beta launch

## Getting Started

### Prerequisites

- Node.js 18+ (LTS recommended)
- pnpm (package manager)
- Supabase CLI (`brew install supabase/tap/supabase` or via npm)
- Expo CLI (for mobile development)

### Installation

```bash
# Clone the repository
git clone https://github.com/gavelinrobert-beep/LiteLists.git
cd LiteLists

# Install dependencies
pnpm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your Supabase and Stripe credentials

# Start local Supabase (optional, for local development)
supabase start

# Run the web app
pnpm dev:web

# Run the mobile app (in a separate terminal)
pnpm dev:mobile
```

### Development Commands

```bash
# Install dependencies
pnpm install

# Development
pnpm dev              # Run all apps in development mode
pnpm dev:web          # Run web app only
pnpm dev:mobile       # Run mobile app only

# Build
pnpm build            # Build all apps
pnpm build:web        # Build web app
pnpm build:mobile     # Build mobile app

# Linting & Formatting
pnpm lint             # Lint all packages
pnpm format           # Format code with Prettier
```

### Environment Variables

Copy `.env.example` to `.env.local` and fill in the required values:

- `NEXT_PUBLIC_SUPABASE_URL` - Your Supabase project URL
- `NEXT_PUBLIC_SUPABASE_ANON_KEY` - Your Supabase anonymous key
- `SUPABASE_SERVICE_ROLE_KEY` - Supabase service role key (server-side only)
- `STRIPE_SECRET_KEY` - Stripe secret key
- `STRIPE_PUBLISHABLE_KEY` - Stripe publishable key

## Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:

- Setting up your development environment
- Branch naming conventions
- Commit message format
- Pull request process
- Code of conduct

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Built with ❤️ for better collaboration**