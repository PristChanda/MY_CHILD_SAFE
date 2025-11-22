# MY_CHILD_SAFE
World vision hackathon project for the anonymous child abuse reporting App in Zambia and soon to make it worldwide.


🛡️ ChildSafe Zambia
A comprehensive child safety reporting system for Zambia, enabling anonymous incident reporting and coordinated response between NGOs, government agencies, and community organizations.

🌟 Project Overview
ChildSafe Zambia is a technology platform designed to protect children through anonymous reporting and rapid response coordination. The system addresses the critical need for safe, accessible reporting mechanisms for child safety concerns across Zambia.

🎯 Mission
To create a safer environment for Zambia's children by providing secure, anonymous reporting and coordinated response to child safety incidents.

💡 Vision
A Zambia where every child is safe, protected, and has access to immediate help when needed.

🏗️ Architecture
This project consists of two main components:



📱 Frontend (Next.js 15)
Framework: Next.js 15 with React 18
Styling: Tailwind CSS with shadcn/ui components
Language: TypeScript
Features: Responsive design, real-time updates, anonymous reporting

🗄️ Backend (Django)
Framework: Django 4.2 with Django REST Framework
Database: SQLite (development), PostgreSQL (production)
Language: Python
Features: JWT authentication, file processing, real-time APIs

🚀 Quick Start
Prerequisites
Node.js 18+ and npm
Python 3.8+ and pip
Git installed

Installation

1 Clone the repository

git clone <repository-url>
cd childsafe-zambia

2 Frontend Setup

# Install dependencies
npm install

# Start development server
npm run dev


childsafe-zambia/
├── 📱 Frontend (Next.js)
│   ├── src/
│   │   ├── app/                 # App Router pages
│   │   ├── components/           # Reusable UI components
│   │   ├── lib/                 # Utilities and configurations
│   │   └── hooks/               # Custom React hooks
│   ├── public/                   # Static assets
│   ├── package.json              # Node.js dependencies
│   └── tailwind.config.ts       # Tailwind configuration
│
├── 🗄️ Backend (Django)
│   ├── childsafe_backend/         # Django project settings
│   ├── accounts/                # User authentication & profiles
│   ├── reports/                 # Incident reporting system
│   ├── api/                    # Dashboard & analytics APIs
│   ├── utils/                   # Image processing & utilities
│   ├── media/                   # File uploads
│   ├── requirements.txt          # Python dependencies
│   └── manage.py               # Django management
│
├── 📚 Documentation
│   ├── README.md                # This file
│   ├── API_DOCUMENTATION.md      # Backend API docs
│   └── PRESENTATION_GUIDE.md    # Presentation guide
│
└── 🎯 Presentation
    ├── childsafe_presentation.html # Interactive presentation
    └── CHILDSAFE_PRESENTATION.md   # Slide content



3 Backend Setup

# Navigate to backend directory
cd childsafe_backend

# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Setup environment
cp .env.example .env
# Edit .env with your configuration

# Database setup
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

# Create sample data (optional)
python manage.py create_sample_data

# Start development server
python manage.py runserver



🌐 Features

🚨 Anonymous Reporting

Secure Form Submission: Anonymous incident reporting with privacy protection
Multi-type Support: Physical abuse, neglect, early marriage, other concerns
Photo Upload: Evidence collection with automatic face blurring
Location Services: GPS-based location with manual override
Urgency Classification: Smart triage system for response prioritization

👥 User Management

Role-based Access: Administrator, Government, NGO roles
Secure Authentication: JWT-based login with session management
Profile Management: User profiles with organization information
Activity Tracking: Comprehensive audit logs

📊 Administrative Dashboard

Real-time Statistics: Live metrics and performance indicators
Case Management: Report assignment, status tracking, resolution
Geographic Visualization: Interactive maps showing incident locations
Multi-agency Coordination: Shared workspace for different organizations

🔒 Security & Privacy

End-to-end Encryption: All communications encrypted
Data Anonymization: Reporter identities protected
Face Blurring: Automatic privacy protection in photos
Access Control: Role-based permissions and audit trails


📱 Frontend Features

🎨 User Interface

Responsive Design: Works on desktop, tablet, and mobile
Modern Components: Built with shadcn/ui component library
Accessibility: WCAG compliant design
Multi-language Support: English with framework for local languages

🔄 Real-time Updates

Live Dashboard: Real-time statistics and updates
WebSocket Support: Instant notifications for new reports
Offline Capability: Progressive Web App features
Performance Optimization: Fast loading and smooth interactions


🗄️ Backend Features

🚀 API Architecture

RESTful Design: Clean, well-documented API endpoints
JWT Authentication: Secure token-based authentication
File Processing: Image upload with automatic processing
Rate Limiting: Protection against abuse


📊 Data Management

Relational Database: Structured data with relationships
Search & Filtering: Advanced filtering and search capabilities
Analytics Engine: Comprehensive reporting and insights
Backup & Recovery: Automated data protection

🔧 Development

🛠️ Tech Stack

Frontend

Next.js 15: React framework with App Router
TypeScript: Type-safe development
Tailwind CSS: Utility-first CSS framework
shadcn/ui: Modern component library
Lucide React: Icon library

Backend

Django 4.2: Python web framework
Django REST Framework: API development
PostgreSQL: Production database
JWT: Authentication tokens
Pillow: Image processing
Redis: Caching and session storage
