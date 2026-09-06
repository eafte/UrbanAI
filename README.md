# UrbanAI - Smart City Management Platform

![UrbanAI Logo](https://img.shields.io/badge/UrbanAI-Smart%20City%20Platform-0077B6)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-0.1.0-green.svg)
![Next.js](https://img.shields.io/badge/Next.js-15.3.3-black)
![React](https://img.shields.io/badge/React-18.3.1-61DAFB)

## 🌆 Overview

UrbanAI is a comprehensive urban planning and visualization platform that leverages artificial intelligence to provide data-driven insights for smart city management. The platform offers real-time analytics, predictive modeling, and interactive visualizations to help urban planners, city administrators, and stakeholders make informed decisions.

## ✨ Key Features

- **Interactive Dashboard** - Visualize urban data with dynamic charts and maps
- **AI-Powered Analytics** - Leverage machine learning for predictive urban planning
- **Traffic Management** - Real-time traffic analysis and simulation
- **Resource Optimization** - Monitor and optimize city resource allocation
- **Environmental Impact** - Track green spaces and environmental metrics
- **Weather Integration** - Access weather insights and forecasting
- **3D Visualization** - Interactive 3D models for urban planning scenarios
- **Multi-language Support** - Internationalization with i18next
- **Authentication System** - Secure user authentication and role-based access
- **Data Export** - Export reports and data in various formats

## 🛠️ Technology Stack

- **Frontend**: React 18, Next.js 15
- **Styling**: Tailwind CSS, Tremor, Radix UI
- **Maps & Visualization**: Leaflet, React Three Fiber, Recharts, Chart.js
- **AI Integration**: OpenAI
- **Authentication**: JWT, bcrypt
- **Database**: Prisma ORM with SQLite (configurable for MySQL)
- **Internationalization**: i18next
- **Deployment**: Docker, Nginx

## 📋 Prerequisites

- Node.js 18.x or higher
- npm or yarn
- Git

## 🚀 Getting Started

### Local Development

1. **Clone the repository**

   ```bash
   git clone https://github.com/eafte/UrbanAI.git
   cd UrbanAI
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env.local` file with the following:

   ```
   DEEPSEEK_API_KEY=your_deepseek_api_key
   METEOSOURCE_API_KEY=your_meteosource_api_key
   OPENWEATHER_API_KEY=your_openweather_api_key
   VISUAL_CROSSING_API_KEY=your_visual_crossing_api_key
   NEXT_PUBLIC_APP_URL=http://localhost:3000
   ```

4. **Set up the database**

   ```bash
   npm run prisma:generate
   npm run prisma:migrate
   npm run prisma:seed
   ```

5. **Start the development server**

   ```bash
   npm run dev
   ```

6. **Open [http://localhost:3000](http://localhost:3000) in your browser**

### Docker Deployment

1. **Build and run with Docker Compose**

   ```bash
   docker-compose up -d
   ```

2. **Access the application at [http://localhost:3000](http://localhost:3000)**

## 🔄 CI/CD and Deployment

### Automated Deployment

Use the included deployment script:

```bash
./deploy.sh
```

This script:

- Pulls latest changes
- Installs dependencies
- Builds the application
- Creates a version tag (format: `vYYYY.MM.DD-HHMM`)
- Deploys the application

### Manual Deployment

1. **Build the application**

   ```bash
   npm run build
   ```

2. **Start the production server**
   ```bash
   npm run start
   ```

## 📊 Project Structure

```
urbanai-project/
├── src/                      # Source code
│   ├── app/                  # Next.js app directory
│   │   ├── (auth)/           # Authentication routes
│   │   ├── (dashboard)/      # Dashboard layout routes
│   │   ├── dashboard/        # Dashboard main components
│   │   └── api/              # API routes
│   ├── components/           # Reusable components
│   ├── contexts/             # React contexts
│   ├── db/                   # Database utilities
│   ├── lib/                  # Library code
│   ├── services/             # Service integrations
│   ├── types/                # TypeScript types
│   └── utils/                # Utility functions
├── prisma/                   # Prisma schema and migrations
├── public/                   # Static assets
├── nginx/                    # Nginx configuration
├── LICENSE                   # MIT License
├── docker-compose.yml        # Docker Compose configuration
└── Dockerfile                # Docker configuration
```

## 🔐 Authentication and Authorization

UrbanAI implements a secure authentication system with JWT tokens and role-based access control:

- **User Roles**: Admin, Planner, Analyst, Viewer
- **Session Management**: Secure JWT-based sessions
- **Password Security**: bcrypt hashing for secure password storage

## 🌐 API Documentation

The platform provides a comprehensive API for integration with other systems:

- **Authentication API**: `/api/auth/*`
- **Projects API**: `/api/projects/*`
- **Analytics API**: `/api/analytics/*`
- **Data API**: `/api/data/*`

## 🤝 Contributing

### Project Contributor

- **Md Mahfujur Rahman Rakib** ([Rakib-codee](https://github.com/Rakib-codee)) — Managed the full coding and development side of the project.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the [MIT License](./LICENSE).

## 📧 Contact

For questions or support, please contact [nexgendev45@gmail.com](mailto:nexgendev45@gmail.com)
