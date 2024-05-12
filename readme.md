# api.blogworks.ai
Interface website for long-running AI API blogging tools






## Technology Stack

### Frontend
- **Astro**: Handles SSR and static generation for efficient, scalable web applications.
- **TailwindCSS**: For rapid, responsive UI development.
- **Svelte**: For client-side reactive components, enhancing interactivity.

### Backend
- **Firebase Functions**: Manages long-running backend processes essential for AI-driven features.
- **Firebase Hosting**: Hosts both static and dynamic content, fully integrated within the Firebase ecosystem.
- **Firebase Firestore**: Real-time database for user data, settings, and API usage metrics.
- **Stripe**: Processes payments and manages subscriptions.

### Authentication and Notifications
- **Lucia**: Implements one-tap login functionality, enhancing user authentication flow.
- **Firebase Notifications**: Manages and sends email notifications regarding account activity, support updates, and billing information.

### DevOps
- **GitHub**: Provides version control and repository hosting, with collaborative tools for development.

### Analytics
- **Google Analytics**: Tracks and analyzes user interaction data for optimization.

## Sitemap Plan

### Public Pages
- `/`: Landing page with service overview, login, and sign-up.
- `/features`: Details on available API services.
- `/pricing`: Subscription tiers and pricing information.

### User Dashboard
- `/dashboard`: Displays statistics, recent activity, and quick links.
    - `/dashboard/settings`: User profile and API key management.
    - `/dashboard/api`: API usage statistics and testing.
    - `/dashboard/billing`: Stripe integration for payment and invoice management.
    - `/dashboard/support`: Support ticket submission and status tracking.

### Admin Area
- `/admin`: Central dashboard with platform analytics and user management.
    - `/admin/users`: User management functionalities including roles and bans.
    - `/admin/analytics`: Usage and financial metrics for APIs and revenue.
    - `/admin/support`: Manage and respond to user support tickets and project requests.
