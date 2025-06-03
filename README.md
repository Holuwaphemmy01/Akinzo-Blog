# Akinzo Blog Platform

A full-featured blogging platform built with the MERN stack (MongoDB, Express.js, React, Node.js).  
Features integrated AI-powered content generation and cloud image storage using [ImageKit.io](https://imagekit.io/).

## Features

- 📝 Create, edit, and delete blog posts
- 🔒 User authentication & authorization (JWT)
- 🖼️ Image uploads & storage via ImageKit
- 🤖 AI content generation for blog posts.
- 🗂️ Category & tag management
- 💬 Commenting system
- 📊 Dashboard & analytics (optional)
- ⚡ Responsive React frontend (with hooks & context)
- 🚀 RESTful API with Express & MongoDB
- 🛡️ Secure password hashing & user roles

---

## Tech Stack

- **Frontend:** React, Redux/Context API, Axios, React Router, TailwindCSS/Bootstrap/Material-UI
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (with Mongoose ORM)
- **AI Integration:** Gemini
- **Image Upload:** ImageKit.io SDK
- **Authentication:** JWT (JSON Web Tokens)
- **Others:** Dotenv, CORS

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/your-blog-platform.git
cd quickblog
```

### 2. Setup Environment Variables

Create a `.env` file in the root (`/server`) with the following (example):

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
OPENAI_API_KEY=your_openai_api_key
```

### 3. Install Dependencies

**Backend:**
```bash
cd server
npm install
```

**Frontend:**
```bash
cd ../client
npm install
```

### 4. Run the App

**Backend:**
```bash
npm run server
```

**Frontend:**
```bash
npm run dev
```

---

## Usage

- Log in as a user or admin
- Create and format blog posts
- Upload images (stored in ImageKit)
- Use the "Generate with AI" feature to auto-generate post content
- Manage categories, tags, and comments

---

## API Endpoints

| Method | Endpoint                 | Description               |
|--------|--------------------------|---------------------------|
| POST   | `/api/auth/register`     | Register new user         |
| POST   | `/api/auth/login`        | User login                |
| POST   | `/api/posts`             | Create new post           |
| GET    | `/api/posts`             | Get all posts             |
| GET    | `/api/posts/:id`         | Get single post           |
| PUT    | `/api/posts/:id`         | Update post               |
| DELETE | `/api/posts/:id`         | Delete post               |
| POST   | `/api/upload`            | Upload image to ImageKit  |
| POST   | `/api/ai/generate`       | Generate content with AI  |
| ...    | ...                      | More endpoints as needed  |

---

## Integrations

### ImageKit

- Handles all image uploads and CDN delivery
- Configure your ImageKit credentials in `.env`

### AI Content Generation

- Uses OpenAI or Gemini API for generating blog content
- Add your API key in `.env`
- Accessible via the "Generate with AI" button in post editor

---

## Folder Structure

```
/client      # React frontend
/server      # Node.js + Express backend
/models      # Mongoose models
/routes      # Express routes
/controllers # Route handlers
/middleware  # Auth & error handling
/utils       # Utility functions (AI, ImageKit, etc.)
.env         # Environment variables
```

---

## Deployment

- Deploy backend (server) to [Render](https://render.com), [Heroku](https://heroku.com), or [Vercel](https://vercel.com)
- Deploy frontend (client) to [Vercel](https://vercel.com), [Netlify](https://netlify.com), or [Render](https://render.com)

---

## Contributing

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## License

[MIT](LICENSE)

---

## Credits

- MERN Stack Community
- [ImageKit.io](https://imagekit.io/)
- [OpenAI](https://openai.com/) / [Google Gemini](https://ai.google.dev/gemini)
