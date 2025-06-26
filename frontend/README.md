# Oktana AI Challenge Frontend

A beautiful, modern chat interface built with Next.js that integrates with FastAPI backend deployed as Vercel Functions.

## Features

- 🎨 **Beautiful Dark UI** - Purple theme with high contrast design
- 💬 **Real-time Chat** - Stream responses from OpenAI GPT models
- ⚙️ **Configurable Settings** - Easy API key and system message management
- 📱 **Responsive Design** - Works perfectly on desktop and mobile
- 🚀 **Fast Performance** - Built with Next.js for optimal speed
- ☁️ **Serverless Backend** - FastAPI deployed as Vercel Functions

## Prerequisites

- Node.js 18+ installed
- Vercel CLI (optional, for deployment)

## Quick Start

1. **Install Dependencies**
   ```bash
   cd frontend
   npm install
   ```

2. **Start the Development Server**
   ```bash
   npm run dev
   ```

3. **Open Your Browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

4. **Configure Your API Key**
   - Click the settings icon (⚙️) in the top right
   - Enter your OpenAI API key
   - Optionally customize the system message
   - Start chatting!

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

### Project Structure

```
frontend/
├── app/                 # Next.js app directory
│   ├── globals.css     # Global styles
│   ├── layout.tsx      # Root layout
│   └── page.tsx        # Main chat interface
├── package.json        # Dependencies and scripts
├── tailwind.config.js  # Tailwind CSS configuration
├── next.config.js      # Next.js configuration
└── tsconfig.json       # TypeScript configuration
```

## Backend Integration

This frontend connects to the FastAPI backend deployed as Vercel Functions. The API is automatically deployed alongside the frontend when you deploy to Vercel.

### Local Development
For local development, the frontend will connect to `http://localhost:8000` if you have the FastAPI backend running locally.

### Production
In production, the frontend automatically connects to the Vercel Functions API at `/api/chat`.

## Deployment

This project is optimized for deployment on Vercel with both frontend and backend:

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically - both frontend and API functions will be deployed

The deployment includes:
- **Frontend**: Next.js app
- **Backend**: FastAPI as Vercel Functions
- **Automatic routing**: API calls are routed to the correct functions

## Customization

### Colors
The app uses a purple theme as specified in the design rules. You can customize colors in `tailwind.config.js`.

### Styling
All styles are built with Tailwind CSS. The main component is in `app/page.tsx`.

## Troubleshooting

- **API Connection Issues**: Ensure your Vercel deployment includes the API functions
- **TypeScript Errors**: Run `npm install` to ensure all dependencies are installed
- **Styling Issues**: Make sure Tailwind CSS is properly configured

## License

This project is part of the Oktana AI Challenge.