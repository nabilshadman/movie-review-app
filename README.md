# Movies Review Database

A full-stack web application for movie reviews leveraging **IBM Cloud** services, featuring sentiment analysis through Natural Language Understanding (NLU) and Cloudant database integration.

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## 🎯 Features

- **Movie Reviews Management**: Create and browse movie reviews
- **Sentiment Analysis**: Automated sentiment analysis of reviews using IBM Watson NLU
- **Data Persistence**: NoSQL data storage with IBM Cloudant
- **Modern UI**: Clean interface built with Bulma CSS framework
- **Internationalization**: Multi-language support with jQuery.i18n
- **Security**: XSS protection and input validation

## 🛠️ Technology Stack

- **Backend**: Node.js, Express.js
- **Frontend**: EJS, Bulma CSS, jQuery
- **Database**: IBM Cloudant
- **AI/ML**: IBM Watson Natural Language Understanding
- **Cloud**: IBM Cloud Platform

## 📋 Prerequisites

- Node.js 12.x or higher
- IBM Cloud account
- IBM Cloudant service instance
- IBM Watson NLU service instance

## 🚀 Getting Started

1. Clone the repository
```bash
git clone https://github.com/yourusername/movies-review-database.git
cd movies-review-database
```

2. Install dependencies
```bash
npm install
```

3. Configure environment variables
```bash
cp .env.sample .env
# Edit .env with your IBM Cloud service credentials
```

4. Start the server
```bash
npm start
```

The application will be available at `http://localhost:8080`

## 🔧 Configuration

The application requires the following environment variables:

```bash
NLU_APIKEY=your_nlu_api_key
NLU_URL=your_nlu_service_url
CLOUDANT_API=your_cloudant_api_key
CLOUDANT_URL=your_cloudant_url
```

## 📁 Project Structure
```
movies-review-database/
├── server.js              # Application entry point
├── utils/                 # Utility functions and strings
├── views/                 # EJS templates and static assets
│   ├── css/              # Stylesheets
│   ├── js/               # Client-side JavaScript
│   └── *.ejs             # Page templates
└── package.json          # Project dependencies
```

## 🔐 IBM Cloud Services

### Cloudant NoSQL DB
- Document-based database for storing reviews
- Automatic replication and data sync
- REST API for data access

### Natural Language Understanding
- Sentiment analysis of review text
- Real-time text processing
- Advanced linguistic analysis

## 🌐 Deployment

### IBM Cloud
```bash
ibmcloud cf push
```

### Docker
```bash
docker build -t movies-review-app .
docker run -p 8080:8080 movies-review-app
```

## 💡 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/enhancement`)
3. Commit changes (`git commit -am 'Add enhancement'`)
4. Push to branch (`git push origin feature/enhancement`)
5. Create Pull Request

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🔗 Resources

- [IBM Cloud Documentation](https://cloud.ibm.com/docs)
- [Cloudant Documentation](https://cloud.ibm.com/docs/Cloudant)
- [Watson NLU Documentation](https://cloud.ibm.com/docs/natural-language-understanding)
- [Express.js Guide](https://expressjs.com/)
- [EJS Documentation](https://ejs.co/)

## 📞 Support

For support and questions, please [open an issue](https://github.com/yourusername/movies-review-database/issues).
