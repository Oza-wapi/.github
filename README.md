# 🌍 Oza Wapi

**Oza Wapi** is a comprehensive social platform and token economy system designed for the Democratic Republic of Congo (DRC). It combines social networking, location-based services, event management, and a robust token reward system to create an engaging digital ecosystem.

## ✨ Features

### 🏗️ **Core Platform**
- **Multi-platform Support**: Web, mobile (iOS/Android), and admin dashboard
- **Real-time Communication**: Live chat, notifications, and activity feeds
- **Location Services**: Check-ins, venue discovery, and geographic analytics
- **Event Management**: Create, manage, and participate in local events
- **Content Sharing**: Posts, media sharing, and social interactions

### 🪙 **Token Economy**
- **Oza Token System**: Earn tokens through platform engagement
- **Reward Mechanisms**: Check-ins, event participation, referrals, and social activities
- **Token Conversion**: Exchange tokens for CDF (Congolese Franc)
- **Referral Program**: Multi-level referral system with token rewards
- **Gamification**: Streaks, achievements, and leaderboards

### 🛡️ **Security & Moderation**
- **Role-Based Access Control (RBAC)**: Granular permissions system
- **Content Moderation**: Automated and manual content review
- **Security Monitoring**: Real-time threat detection and response
- **Data Privacy**: GDPR-compliant data handling and user privacy controls

### 📊 **Analytics & Insights**
- **Real-time Dashboard**: Comprehensive admin analytics
- **User Engagement Metrics**: Activity tracking and engagement analysis
- **Geographic Analytics**: Location-based insights and heatmaps
- **Revenue Analytics**: Token economy and financial metrics

## 🏛️ **Architecture**

### **Monorepo Structure**
```
oza-wapi/
├── apps/
│   ├── web/           # Next.js web application
│   ├── native/        # React Native mobile app (Expo)
│   ├── admin/         # Admin dashboard (Next.js)
│   └── landing/       # Marketing landing page
├── packages/
│   ├── backend/       # Convex backend (schema, functions, auth)
│   ├── ui/           # Shared UI components (shadcn/ui)
│   └── utils/        # Shared utilities and types
```

### **Tech Stack**
- **Frontend**: Next.js 14, React Native (Expo), TypeScript
- **Backend**: Convex (real-time database & functions)
- **Authentication**: Better-Auth with multi-provider support
- **Styling**: TailwindCSS, shadcn/ui components
- **Build System**: Turborepo for optimized monorepo builds
- **Package Manager**: Bun for fast dependency management

## 🚀 **Getting Started**

### **Prerequisites**
- Node.js 18+ or Bun
- Expo CLI (for mobile development)
- Convex account

### **Installation**

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-org/oza-wapi.git
   cd oza-wapi
   ```

2. **Install dependencies**
   ```bash
   bun install
   ```

3. **Setup Convex backend**
   ```bash
   bun dev:setup
   ```
   Follow the prompts to create and configure your Convex project.

4. **Start development servers**
   ```bash
   # Start all applications
   bun dev

   # Or start individual apps
   bun dev:web      # Web app (localhost:3000)
   bun dev:admin    # Admin dashboard (localhost:3001)
   bun dev:native   # Mobile app (Expo)
   ```

### **Environment Setup**

Create `.env.local` files in each app directory:

```env
# Convex
CONVEX_DEPLOYMENT=your-deployment-url
NEXT_PUBLIC_CONVEX_URL=your-convex-url

# Authentication
BETTER_AUTH_SECRET=your-auth-secret
BETTER_AUTH_URL=http://localhost:3000

# Optional: Third-party integrations
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
```

## 📱 **Applications**

### **Web App** (`/apps/web`)
- User-facing social platform
- Event discovery and management
- Token wallet and transactions
- Social features and messaging

### **Mobile App** (`/apps/native`)
- Native iOS/Android experience
- Location-based check-ins
- Push notifications
- Offline-first architecture

### **Admin Dashboard** (`/apps/admin`)
- Real-time analytics and monitoring
- User and content moderation
- System health monitoring
- Token economy management

### **Landing Page** (`/apps/landing`)
- Marketing website
- Feature showcase
- User onboarding

## 🗄️ **Database Schema**

### **Core Entities**
- **Users**: Profile management, authentication, preferences
- **Venues**: Locations, check-ins, analytics
- **Events**: Event management, participation, scheduling
- **Posts**: Content sharing, media, interactions
- **Tokens**: Economy system, transactions, rewards

### **Key Features**
- **RBAC System**: Roles, permissions, and access control
- **Moderation**: Content review, reporting, automated filtering
- **Analytics**: User behavior, engagement metrics, geographic data
- **Notifications**: Real-time alerts, push notifications, email

## 🛠️ **Development**

### **Available Scripts**
```bash
# Development
bun dev                 # Start all apps in development
bun dev:web            # Start web app only
bun dev:admin          # Start admin dashboard only
bun dev:native         # Start mobile app only

# Building
bun build              # Build all applications
bun build:web          # Build web app only
bun build:admin        # Build admin dashboard only

# Quality Assurance
bun check-types        # TypeScript type checking
bun lint               # ESLint code linting
bun test               # Run test suites
```

### **Code Quality**
- **TypeScript**: Strict type checking across all packages
- **ESLint**: Consistent code style and best practices
- **Prettier**: Automated code formatting
- **Husky**: Pre-commit hooks for quality gates

## 🌍 **Localization**

Oza Wapi supports multiple languages with focus on:
- **French**: Primary language for DRC
- **Lingala**: Local language support
- **Swahili**: Regional language support
- **English**: International accessibility

## 🔒 **Security**

### **Authentication & Authorization**
- Multi-factor authentication (MFA)
- OAuth integration (Google, Facebook, etc.)
- Role-based access control (RBAC)
- Session management and security

### **Data Protection**
- End-to-end encryption for sensitive data
- GDPR compliance and data privacy
- Secure token transactions
- Regular security audits

## 📈 **Analytics & Monitoring**

### **Real-time Metrics**
- User engagement and activity
- Token economy performance
- Geographic usage patterns
- System health and performance

### **Business Intelligence**
- Revenue analytics and forecasting
- User behavior analysis
- Market penetration insights
- Growth metrics and KPIs

## 🤝 **Contributing**

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### **Development Workflow**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 **Support**

- **Documentation**: [docs.ozawapi.com](https://docs.ozawapi.com)
- **Community**: [Discord Server](https://discord.gg/ozawapi)
- **Issues**: [GitHub Issues](https://github.com/your-org/oza-wapi/issues)
- **Email**: support@ozawapi.com

## 🗺️ **Roadmap**

### **Phase 1: Core Platform** ✅
- [x] User authentication and profiles
- [x] Basic social features
- [x] Token system foundation
- [x] Admin dashboard

### **Phase 2: Enhanced Features** 🚧
- [ ] Advanced analytics
- [ ] Mobile app optimization
- [ ] Payment integrations
- [ ] API marketplace

### **Phase 3: Scale & Expansion** 📋
- [ ] Multi-country support
- [ ] Enterprise features
- [ ] Third-party integrations
- [ ] Advanced AI features

---

**Built with ❤️ for the Democratic Republic of Congo**

*Empowering communities through technology and token economics.*
