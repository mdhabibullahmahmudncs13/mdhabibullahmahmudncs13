# MD HABIBULLAH MAHMUD - Personal Portfolio

[![Portfolio Website](https://img.shields.io/badge/Visit-Portfolio-blue)](https://www.mdhabibullahmahmud.me/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5)](https://www.linkedin.com/in/md-habibullah-mahmud-3820382a9/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717)](https://github.com/mdhabibullahmahmudncs13)

## 👨‍💻 About Me

I am MD HABIBULLAH MAHMUD, a versatile tech expert from Dhaka, Bangladesh, currently pursuing a Bachelor of Science in Computer Science and Engineering at the National Institute of Textile Engineering and Research (NIT). My focus areas include web development, Python, AI, cybersecurity (ethical hacking), and robotics. I am passionate about building innovative solutions, optimizing digital experiences, and enhancing security in the ever-evolving tech landscape.

---

## 🚀 This Project

A modern, dynamic portfolio website built with SvelteKit frontend and Django REST API backend. Showcasing my skills, experience, and projects with a secure admin panel for content management.

## 📁 Project Structure

```
portfolio-svelte-django/
├── backend/                 # Django REST API
│   ├── api/                # API app with models, views, serializers
│   ├── portfolio_backend/  # Django project settings
│   ├── manage.py
│   └── requirements.txt
│
├── frontend/               # SvelteKit app
│   ├── src/
│   │   ├── lib/           # Utilities, types, API client
│   │   └── routes/        # SvelteKit routes
│   ├── package.json
│   └── svelte.config.js
│
└── README.md
```

## 🚀 Features

- **Public Portfolio Pages**: Hero, Skills, Projects, Experience, Certifications, Contact, Blog
- **Admin Panel**: Secure content management at `/xenon` (login at `/whoami`)
- **Contact Form**: Message submissions stored in database
- **File Uploads**: Images, videos, PDFs support
- **RESTful API**: Django REST Framework with JWT authentication
- **Modern UI**: TailwindCSS, dark theme, responsive design

## 🛠️ Tech Stack

**Frontend:**
- SvelteKit 2.0
- TypeScript
- TailwindCSS
- Vite

**Backend:**
- Django 4.2+
- Django REST Framework
- Simple JWT
- PostgreSQL (production) / SQLite (development)

## 📦 Installation

### Backend Setup

```bash
cd backend

# Install dependencies (create virtual environment first if needed)
pip install -r requirements.txt

# Copy environment file
cp .env.example .env

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Create superuser for admin access
python manage.py createsuperuser

# Run development server
python manage.py runserver
```

The API will be available at `http://localhost:8000/api/`

### Frontend Setup

```bash
cd frontend

# Install dependencies
npm install

# Copy environment file
cp .env.example .env

# Run development server
npm run dev
```

The frontend will be available at `http://localhost:5173`

## 🔐 Authentication

1. Create a superuser in Django: `python manage.py createsuperuser`
2. Login at `/whoami` using your credentials
3. Access admin panel at `/xenon`

## 📡 API Endpoints

### Public Endpoints
- `GET /api/hero/` - Get hero section data
- `GET /api/skills/` - List all skills
- `GET /api/projects/` - List all projects
- `GET /api/experience/` - List experience
- `GET /api/certifications/` - List certifications
- `GET /api/contact/` - Get contact information
- `POST /api/messages/` - Submit contact form
- `GET /api/blog/` - List published blog posts

### Admin Endpoints (Require JWT Token)
- All POST, PUT, PATCH, DELETE operations
- `GET /api/messages/` - View all messages
- POST `/api/token/` - Obtain JWT token
- POST `/api/token/refresh/` - Refresh JWT token

## 💼 Professional Background

### Technical Skills
- **Languages**: Python, JavaScript, TypeScript
- **Web Development**: HTML, CSS, JavaScript, Responsive Design
- **Frontend**: SvelteKit, React basics, TailwindCSS
- **Backend**: Django, Django REST Framework
- **Databases**: PostgreSQL, SQLite
- **Cybersecurity & Ethical Hacking**: Network security, penetration testing basics
- **AI & Machine Learning**: Basic ML concepts and applications
- **Robotics**: Embedded systems, Arduino

### Specializations
- **Digital Marketing**: SEO, Social Media Marketing, Digital Communications
- **Full-Stack Web Development**: from frontend to backend architecture

### Experience

**Digital Marketing Intern** | Aurora Innovative  
*August 2023 - January 2024 (6 months)*
- Implemented digital marketing strategies and SEO optimization
- Worked on social media and digital marketing communications
- Contributed to content marketing campaigns

### Education

**Bachelor of Science in Computer Science and Engineering**  
National Institute of Textile Engineering and Research (NIT)  
*October 2023 - Present*

### Featured Projects

**Education Exam System - Dig The Data 3.0**
- Comprehensive Event and Exam Management System for competitive quizzes
- Role: Frontend Developer
- Features: User authentication, team management, quiz scoring, leaderboards
- Tech: Django, Django REST Framework, HTML, CSS, JavaScript
- Used by: NIT Computer Club (NCC)
- [View Repository](https://github.com/mdhabibullahmahmudncs13/education-exam-system)

**Personal Portfolio Website** (This Project)
- Modern portfolio with SvelteKit frontend and Django REST backend
- Features: Admin panel, SEO-optimized pages, contact forms, file uploads
- Tech: SvelteKit, TypeScript, TailwindCSS, Django, PostgreSQL

### Current Focus

Actively developing expertise in:
- Advanced Python programming
- Full-stack web development with modern frameworks
- Artificial Intelligence and Machine Learning applications
- Cybersecurity and ethical hacking
- Deployment and DevOps practices

### Open to Opportunities

I'm actively seeking opportunities in:
- Web development and full-stack projects
- Django/Python backend development
- AI and machine learning applications
- Cybersecurity initiatives
- Robotics and embedded systems
- Digital transformation projects

## 🌐 Environment Variables

### Backend (.env)
```
SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
CORS_ALLOWED_ORIGINS=http://localhost:5173,http://127.0.0.1:5173
```

### Frontend (.env)
```
PUBLIC_API_URL=http://localhost:8000/api
```

## 🚢 Deployment

### Backend (Railway/Render/Heroku)
1. Set environment variables
2. Use PostgreSQL database
3. Run `python manage.py collectstatic`
4. Set `DEBUG=False` in production

### Frontend (Vercel)
1. Connect GitHub repository
2. Set `PUBLIC_API_URL` to your backend URL
3. Deploy

## 📝 Models

- **Hero**: Portfolio owner information
- **Skill**: Technical skills with proficiency levels
- **Project**: Portfolio projects with images/videos
- **Experience**: Work experience timeline
- **Certification**: Certifications and courses
- **Contact**: Contact information
- **Message**: Contact form submissions
- **BlogPost**: Blog articles with markdown support

## 🔧 Development

### Run Backend Tests
```bash
cd backend
python manage.py test
```

### Build Frontend
```bash
cd frontend
npm run build
```

## 📄 License

MIT License

## 👤 Author

**MD HABIBULLAH MAHMUD**  
Tech Professional | Web Developer | Computer Science Student  

- **Email**: mdhabibullahmahmudncs13@gmail.com
- **Portfolio**: [mdhabibullahmahmud.me](https://www.mdhabibullahmahmud.me/)
- **LinkedIn**: [MD Habibullah Mahmud](https://www.linkedin.com/in/md-habibullah-mahmud-3820382a9/)
- **GitHub**: [mdhabibullahmahmudncs13](https://github.com/mdhabibullahmahmudncs13)
