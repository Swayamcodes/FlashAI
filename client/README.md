# FlashAI

A modern, full-stack AI-powered SaaS application that provides powerful tools for content creation, image processing, and resume analysis. Built with React, Node.js, and cutting-edge AI technologies.



## ✨ Features

### 🤖 AI Content Generation
- **Article Generator**: Create full-length articles on any topic
- **Blog Title Generator**: Generate catchy, SEO-friendly blog titles
- **Creative Writing**: AI-powered story and content creation
- **Content Optimization**: Enhance existing content with AI suggestions

### 🎨 Image AI Tools
- **AI Image Generation**: Create unique images from text descriptions
- **Background Removal**: Instantly remove backgrounds from images
- **Object Removal**: Smart object detection and removal
- **Image Enhancement**: AI-powered image quality improvements

### 📄 Resume Analysis
- **Smart Resume Review**: AI-powered resume analysis and feedback
- **ATS Optimization**: Ensure your resume passes applicant tracking systems
- **Skill Gap Detection**: Identify missing skills for target roles
- **Personalized Suggestions**: Get tailored recommendations for improvement

### 👤 User Features
- **Personal Dashboard**: Centralized workspace for all AI tools
- **Usage Tracking**: Monitor your AI tool usage and history
- **Secure Authentication**: Industry-standard auth with Clerk
- **Responsive Design**: Beautiful UI that works on all devices

## 🛠️ Tech Stack

### Frontend
- **React 19** - Modern UI library with latest features
- **Vite** - Lightning-fast build tool
- **Tailwind CSS** - Utility-first CSS framework
- **React Router** - Client-side routing
- **Axios** - HTTP client for API requests

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **PostgreSQL** - Relational database via Neon
- **Multer** - File upload handling
- **CORS** - Cross-origin resource sharing

### AI & Services
- **OpenAI API** - GPT models for content generation
- **Cloudinary** - Image processing and storage
- **Clerk** - Authentication and user management

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ installed
- PostgreSQL database (Neon recommended)
- OpenAI API key
- Cloudinary account
- Clerk account

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/FlashAI.git
cd ai-saas-platform
```

2. **Install frontend dependencies**
```bash
cd client
npm install
```

3. **Install backend dependencies**
```bash
cd ../server
npm install
```

### Environment Variables

Create a `.env` file in the `server` directory:

```env
# OpenAI
OPENAI_API_KEY=your_openai_api_key

# Cloudinary
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Database
DATABASE_URL=your_neon_postgresql_url

# Clerk
CLERK_SECRET_KEY=your_clerk_secret_key

# Server
PORT=5000
NODE_ENV=development
```

Create a `.env` file in the `client` directory:

```env
VITE_API_URL=http://localhost:5000
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

### Running the Application

**Start the backend server:**
```bash
cd server
npm run server
```

**Start the frontend (in a new terminal):**
```bash
cd client
npm run dev
```

The application will be available at:
- Frontend: `http://localhost:5173`
- Backend: `http://localhost:5000`

## 📁 Project Structure

```
ai-saas-platform/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Route pages
│   │   ├── services/      # API service functions
│   │   ├── utils/         # Helper functions
│   │   ├── App.jsx        # Main app component
│   │   └── main.jsx       # Entry point
│   ├── public/            # Static assets
│   └── package.json
│
├── server/                # Node.js backend
│   ├── routes/            # API routes
│   ├── controllers/       # Route controllers
│   ├── middleware/        # Custom middleware
│   ├── config/            # Configuration files
│   ├── utils/             # Helper functions
│   ├── server.js          # Server entry point
│   └── package.json
│
└── README.md
```

## 🔧 Configuration

### Database Setup

1. Create a PostgreSQL database on [Neon](https://neon.tech)
2. Run migrations (if applicable):
```bash
cd server
npm run migrate
```

### Clerk Setup

1. Create a new application on [Clerk](https://clerk.com)
2. Configure allowed redirect URLs
3. Copy your publishable and secret keys

### OpenAI Setup

1. Sign up at [OpenAI](https://platform.openai.com)
2. Generate an API key
3. Set usage limits and billing

### Cloudinary Setup

1. Create account at [Cloudinary](https://cloudinary.com)
2. Get your cloud name and API credentials
3. Configure upload presets (optional)

## 🎯 Usage

### Content Generation
1. Navigate to the Content Generation section
2. Select your desired tool (Article, Blog Title, etc.)
3. Enter your prompt or topic
4. Click generate and wait for AI response
5. Copy, edit, or regenerate as needed

### Image Processing
1. Go to Image AI Tools
2. Choose your tool (Generate, Remove BG, etc.)
3. Upload image or enter description
4. Process with AI
5. Download or edit result

### Resume Analysis
1. Access Resume Analysis tool
2. Upload your resume (PDF/DOCX)
3. Optionally add job description for targeted analysis
4. Review AI feedback and suggestions
5. Download improved version

## 🚢 Deployment

### Frontend (Vercel)
```bash
cd client
npm run build
# Deploy to Vercel
```

### Backend (Railway/Render)
```bash
cd server
# Deploy to your preferred platform
```

### Environment Variables
Make sure to set all production environment variables in your deployment platform.

## 🔒 Security

- Clerk handles authentication and session management
- API keys stored securely in environment variables
- CORS configured for production domains
- Input validation on all API endpoints
- Rate limiting on AI endpoints (recommended)

## 📝 API Endpoints

### Content Generation
- `POST /api/content/generate-article` - Generate article
- `POST /api/content/generate-title` - Generate blog title

### Image Processing
- `POST /api/image/generate` - Generate image from text
- `POST /api/image/remove-bg` - Remove background
- `POST /api/image/remove-object` - Remove object

### Resume Analysis
- `POST /api/resume/analyze` - Analyze resume
- `POST /api/resume/optimize` - Get optimization suggestions

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🙏 Acknowledgments

- OpenAI for providing powerful AI models
- Clerk for seamless authentication
- Cloudinary for image processing capabilities
- The open-source community

## 📧 Contact

Swayam Shinde - [@raspberrychai_](https://twitter.com/raspberrychai_) - shindeswayam2004@gmail.com

Project Link: [https://github.com/Swayamcodes/FlashAI](https://github.com/yourusername/FlashAI)

---

**Built with ❤️ by Swayam Shinde**