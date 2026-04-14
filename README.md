
🚀 AI-Powered Resume Analyzer & Interview Preparation Platform
📌 Overview
This project is an AI-powered web application that analyzes a candidate’s resume against a job description and generates a detailed interview preparation report.
It uses a hybrid approach combining Machine Learning and Generative AI (Gemini) to provide accurate insights and personalized recommendations.

✨ Features


📄 Upload Resume (PDF supported)


📝 Input Job Description


👤 Add Self Description


📊 Generate Match Score (ML-based)


🧠 Detect Skill Gaps


❓ Generate Technical Interview Questions


💬 Generate Behavioral Questions


📅 Personalized Preparation Plan


📥 Download Resume PDF


🔐 Authentication (Login/Register with JWT)



🧠 How It Works


User provides:


Resume


Job Description


Self Description




ML model analyzes:


Skill extraction


Match score


Skill gaps




Gemini API generates:


Technical questions


Behavioral questions


Preparation plan




Final output:


Match Score


Skill Gaps


Interview Questions


Preparation Plan





🏗️ Tech Stack
Frontend


React (Vite)


Context API


Axios


Backend


Node.js


Express.js


MongoDB (Mongoose)


JWT Authentication


Multer (file upload)


AI 


Google Gemini API (@google/genai)


NLP-based similarity (ML model)



📂 Project Structure
project-root/│├── backend/│   ├── controllers/│   ├── routes/│   ├── services/│   ├── models/│   └── app.js│├── frontend/│   ├── features/│   ├── hooks/│   ├── pages/│   └── services/
⚙️ Setup Instructions
1️⃣ Clone Repository
git clone https://github.com/your-username/your-repo-name.gitcd your-repo-name

2️⃣ Backend Setup
cd backendnpm install
Create .env file:
PORT=3000MONGO_URI=your_mongodb_uriJWT_SECRET=your_secret_keyGOOGLE_GENAI_API_KEY=your_gemini_api_key
Run backend:
npm run dev

3️⃣ Frontend Setup
cd frontendnpm installnpm run dev

🔐 Authentication Flow


User registers or logs in


JWT stored in cookies


Protected routes require authentication


/get-me fetches logged-in user



📊 API Endpoints
Auth


POST /api/auth/register


POST /api/auth/login


GET /api/auth/logout


GET /api/auth/get-me


Interview


POST /api/interview → Generate report


GET /api/interview → Get all reports


GET /api/interview/report/:id → Get report by ID


POST /api/interview/resume/pdf/:id → Download resume PDF



🧪 Sample Flow


Upload resume


Paste job description


Click "Generate Report"


Get:


Match Score


Skill Gaps


Questions


Preparation Plan





💡 Key Highlights


Hybrid AI system (LLM)


Real-world MERN architecture


Secure authentication using cookies


Error handling & fallback system


Scalable design



🚀 Future Enhancements


Advanced NLP skill extraction


Local LLM integration (Ollama/Llama)


Dashboard with analytics


Deployment (Vercel + Render)


Data visualization





⭐ Contribute
Feel free to fork this project and improve it!



