# api.blogworks.ai
Interface website for long-running AI API blogging tools


# Blockworks.ai Setup Instructions

## Initial Setup
- [x] **Create GitHub Repository**: Create a private repository on GitHub named `api.blogworks.ai`.
- [x] **Clone the Repository**: Clone the repository to your local machine using `git clone https://github.com/yourusername/api.blogworks.ai.git`.

## Frontend Setup
### Astro and TailwindCSS
- [x] **Initialize Astro Project**: Run `npm init astro` inside the project directory and follow the setup wizard to create a new Astro project.
- [x] **Install TailwindCSS**: Integrate TailwindCSS by running `npm install -D tailwindcss@latest postcss@latest autoprefixer@latest` and then configure it according to the Astro documentation.
- [x] **Set Up Svelte**: Install Svelte with `npm install svelte` and configure it to work with Astro.

### File Structure
- [x] **Create Directory Structure**: Set up the following directories:
  - `src/`: Contains all source files.
  - `src/components/`: Svelte components.
  - `src/pages/`: Astro pages for static and SSR content.

## Backend Setup
### Firebase Setup
- [ ] **Create Firebase Project**: Through the Firebase Console, create a new project and name it according to your project needs.
- [ ] **Initialize Firebase in your Project**: Run `firebase init` and follow the prompts to set up Firestore, Functions, and Hosting.
- [ ] **Install Firebase SDK**: Run `npm install firebase-admin --save` for backend interactions.

### Firebase Functions
- [ ] **Set Up Functions Directory**: Ensure the `functions/` directory is set up through `firebase init`.
- [ ] **Develop API Functions**: Code your Firebase Functions to handle backend logic such as API requests for translations, narrations, image generation, and other AI-driven features.

## Stripe Integration
- [ ] **Set Up Stripe**: Run `npm install stripe` and configure it for handling payments.
- [ ] **Configure Environment Variables**: Set your Stripe secret key in Firebase Functions environment using `firebase functions:config:set stripe.secret_key="your_secret_key"`.

## Authentication with Lucia
- [ ] **Install Lucia**: Follow the official Lucia documentation to integrate authentication into your Astro project.
- [ ] **Configure Authentication Routes**: Implement routes in Astro for login, logout, and user session management.

## Deployment and Monitoring
### Deploy to Firebase Hosting
- [ ] **Build Astro Project**: Run `npm run build` to generate static files.
- [ ] **Deploy to Firebase Hosting**: Use `firebase deploy` to deploy your site and functions.

### Analytics Setup
- [ ] **Integrate Google Analytics**: Set up Google Analytics by including the tracking code in the Astro pages.

## Final Steps
- [ ] **Review Everything**: Go through the entire setup to ensure everything is configured correctly.
- [ ] **Launch**: Make your initial commit to GitHub and push it using `git add .`, `git commit -m "Initial commit"`, and `git push origin main`.
- [ ] **Monitor**: Regularly check Firebase Console and Google Analytics for insights and ensure all systems are operational.








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
