# Public Opinion Index

## Overview

This is an **open-source** platform that allows the public to poll on **pending government initiatives and bills** in Canada. The platform is designed to be **neutral, transparent, and trustworthy**, leveraging AI to summarize bills and analyze public consensus.

## Features

- **AI-Powered Bill Summaries**: Automatically generated, easy-to-understand breakdowns of legislative initiatives.
- **Public Polling System**: Citizens can vote and express their stance on each bill.
- **Forum Discussions**: A space for discussion, with AI summarizing the general consensus.
- **Open Source & Transparent**: All data, summaries, and discussions are publicly visible.
- **Privacy-Focused**: No personal tracking; user opinions remain anonymous.

## Tech Stack

### **Frontend** (Next.js + TypeScript)

- **Framework**: [Next.js](https://nextjs.org/) (React-based SPA)
- **Styling**: Tailwind CSS
- **State Management**: Local state + API calls
- **Hosting**: Vercel (for now)

### **Backend** (Node.js + Express + PostgreSQL)

- **API Framework**: Express.js
- **Database**: PostgreSQL (hosted on DigitalOcean)
- **Authentication**: OAuth (NextAuth.js)
- **Hosting**: DigitalOcean VPS

### **AI Integration**

- **LLM-powered Bill Summaries**
- **NLP-driven Opinion Analysis in Forums**

## Development Setup

### **1. Clone the Repository**

```sh
git clone https://github.com/qiyundai/poi.git
cd poi
```

### **2. Install Dependencies**

#### Backend

```sh
cd backend
npm install
```

#### Frontend

```sh
cd ../frontend
npm install
```

### **3. Set Up Environment Variables**

#### Backend (`backend/.env`)

```
DATABASE_URL=postgresql://polling_user:securepassword@localhost:5432/gov_polling
PORT=4000
```

#### Frontend (`frontend/.env.local`)

```
NEXT_PUBLIC_API_URL=http://localhost:4000
```

### **4. Run the Application**

#### Start Backend

```sh
cd backend
npm run dev
```

#### Start Frontend

```sh
cd frontend
npm run dev
```

## Contributing

We welcome public contributions! To contribute:

1. Fork the repo.
2. Create a feature branch.
3. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).


