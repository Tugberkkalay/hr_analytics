# 📊 HR Analytics Platform

AI-powered, no-code HR analytics application built with React and Node.js. Upload CSV/Excel files and create custom HR dashboards with category-based metrics.

## Features

✨ **Key Features:**
- 📁 CSV/Excel file upload support
- 🎨 Category-based dashboard configuration (Executive Summary, Performance, etc.)
- 📊 Interactive charts and visualizations
- 🎯 No-code setup - create your own HR metrics categories
- 🚀 Fast and responsive UI

## Tech Stack

### Backend
- **Node.js** with Express.js
- **Multer** for file uploads
- **CORS** for cross-origin requests

### Frontend
- **React 18** for UI
- **Recharts** for data visualization
- **Axios** for API calls
- **React Router** for navigation

## Project Structure

```
hr_analytics/
├── backend/
│   ├── server.js           # Main Express server
│   ├── package.json        # Backend dependencies
│   ├── .env               # Environment variables
│   ├── .gitignore         # Git ignore rules
│   └── uploads/           # Uploaded file storage
│
├── frontend/
│   ├── public/
│   │   └── index.html     # HTML template
│   ├── src/
│   │   ├── index.js       # React entry point
│   │   ├── App.js         # Main app component
│   │   ├── App.css        # App styles
│   │   └── components/
│   │       ├── FileUpload.js     # File upload component
│   │       ├── FileUpload.css    # Upload styles
│   │       ├── Dashboard.js      # Dashboard component
│   │       └── Dashboard.css     # Dashboard styles
│   ├── package.json       # Frontend dependencies
│   └── .gitignore         # Git ignore rules
│
└── README.md              # This file
```

## Getting Started

### Prerequisites
- Node.js (v14+)
- npm or yarn

### Backend Setup

```bash
cd backend
npm install
npm run dev
```

The backend will run on `http://localhost:5000`

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

The frontend will run on `http://localhost:3000`

## Usage

1. **Start Backend**: `npm run dev` in the `backend` folder
2. **Start Frontend**: `npm start` in the `frontend` folder
3. **Upload Data**: Navigate to the upload page and select your CSV/Excel file
4. **Create Categories**: Define HR analytics categories (e.g., "Executive Summary", "Performance")
5. **View Dashboard**: Your data will be processed and visualizations generated

## CSV/Excel Format Example

```
Employee_ID,Employee_Name,Department,Salary,Performance_Score,Hire_Date,Status
1,John Doe,Engineering,50000,85,2020-01-15,Active
2,Jane Smith,Marketing,45000,92,2019-06-20,Active
3,Bob Johnson,Sales,55000,78,2021-03-10,Active
```

## Supported File Types
- CSV (.csv)
- Excel (.xlsx, .xls)

## API Endpoints

### Health Check
```
GET /api/health
```

### File Upload
```
POST /api/upload
Content-Type: multipart/form-data

Parameters:
- file: CSV or Excel file
```

## Future Enhancements

- 📈 Advanced data visualization options
- 🔐 User authentication
- 💾 Database integration (PostgreSQL, MongoDB)
- 🌐 API integrations (Salesforce, HR software)
- 🤖 AI-powered insights using LLM
- 📊 Real-time data syncing
- 🎨 Custom widget builder

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the MIT License.

## Support

For issues, questions, or suggestions, please open an issue on GitHub.

---

**Built with ❤️ for HR Analytics**