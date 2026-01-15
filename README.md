# LiteLists

**Real-time collaborative lists for roommates and small groups**

LiteLists is a simple, fast, and intuitive app that helps roommates and small groups stay organized with shared lists. Whether it's groceries, chores, or household tasks, LiteLists keeps everyone on the same page in real-time.

## ✨ Features

- 📝 **Create and share lists** - Grocery lists, todo lists, chore assignments, and more
- 🔄 **Real-time sync** - Changes appear instantly for all collaborators
- 👥 **Group collaboration** - Perfect for roommates, families, and small teams
- 📱 **Cross-platform** - Works seamlessly on web and mobile devices
- 🎨 **Clean & simple** - Focused on what matters: your lists

## 🛠️ Tech Stack

LiteLists is built with modern, reliable technologies:

- **Frontend (Web)**: [Next.js](https://nextjs.org/) - React framework with SSR and optimal performance
- **Frontend (Mobile)**: [Expo](https://expo.dev/) - React Native development platform for iOS and Android
- **Backend & Database**: [Supabase](https://supabase.com/) - Open-source Firebase alternative with PostgreSQL
- **Real-time**: Supabase Realtime - WebSocket-based live updates
- **Authentication**: Supabase Auth - Secure user management
- **Deployment**: Vercel (web) + Expo EAS (mobile)

## 🎯 MVP Scope

The Minimum Viable Product focuses on core functionality:

### Included in MVP
- ✅ User authentication (email/password)
- ✅ Create, edit, and delete lists
- ✅ Add, check off, and remove items
- ✅ Invite collaborators to lists via email or shareable link
- ✅ Real-time synchronization across devices
- ✅ Basic mobile app (iOS and Android)
- ✅ Responsive web application

### Post-MVP Features
- 🔜 Push notifications for list updates
- 🔜 Categories and tags for items
- 🔜 Recurring lists (weekly groceries, etc.)
- 🔜 Item assignment to specific users
- 🔜 In-app messaging or comments
- 🔜 Dark mode

## 🗺️ Roadmap

### Phase 1: Foundation (Current)
- Set up monorepo structure
- Initialize Next.js and Expo projects
- Configure Supabase backend
- Implement basic authentication

### Phase 2: Core Features
- List CRUD operations
- Item management
- Real-time synchronization
- Basic UI/UX implementation

### Phase 3: Collaboration
- User invitations and sharing
- Multi-user list access
- Permissions management

### Phase 4: Polish & Launch
- Mobile app optimization
- Performance improvements
- User testing and feedback
- Production deployment
- App store submissions

### Phase 5: Growth
- Advanced features from post-MVP list
- Analytics and insights
- User feedback integration
- Platform expansion

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm/yarn/pnpm
- Expo CLI (for mobile development)
- Supabase account (free tier available)

### Installation

```bash
# Clone the repository
git clone https://github.com/gavelinrobert-beep/LiteLists.git
cd LiteLists

# Install dependencies (when available)
npm install

# Set up environment variables
cp .env.example .env.local
# Add your Supabase credentials to .env.local

# Run the web app
npm run dev:web

# Run the mobile app
npm run dev:mobile
```

## 🤝 Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details on:
- Code of conduct
- Development workflow
- Submitting pull requests
- Coding standards

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

Questions or suggestions? Open an issue or reach out to the maintainers.

---

**Built with ❤️ for better collaboration**