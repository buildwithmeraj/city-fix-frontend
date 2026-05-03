# CityFix Frontend

CityFix is a community issue reporting platform where users can report city problems, track progress, and contribute funds to clean-up/fix campaigns.

Live site: [https://city-fix.pages.dev](https://city-fix.pages.dev)

## Features

- User authentication with Firebase (email/password + Google login)
- Report, browse, and filter public city issues
- Private user dashboard for personal issues and contributions
- Contribution flow with progress tracking
- Download contribution report as PDF
- Fully responsive UI

## Tech Stack

- React 19 + Vite
- React Router v7
- Tailwind CSS + DaisyUI
- Firebase Authentication
- Axios
- jsPDF + jsPDF-AutoTable
- react-hot-toast

## Project Setup

### Prerequisites

- Node.js 18+ (recommended: latest LTS)
- npm

### Installation

```bash
npm install
```

### Environment Variables

Create a `.env` file in the project root and add:

```env
VITE_apiKey=your_firebase_api_key
VITE_authDomain=your_firebase_auth_domain
VITE_projectId=your_firebase_project_id
VITE_storageBucket=your_firebase_storage_bucket
VITE_messagingSenderId=your_firebase_messaging_sender_id
VITE_appId=your_firebase_app_id
```

### Run Locally

```bash
npm run dev
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Create production build
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint

## Project Structure

- `src/pages` - Route-level pages
- `src/components` - Shared and UI components
- `src/contexts` - Context providers
- `src/hooks` - Reusable hooks and API instance
- `src/routes` - Routing and private route guard

## Notes

- Backend API is currently configured in `src/hooks/axiosInstance.jsx`.
- Authentication is initialized from `src/firebase/firebase.config.js`.
