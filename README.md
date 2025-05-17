# Budget Tracker API

A RESTful API for managing personal finances, built with Node.js, Express, and MongoDB.

## Live API
API Base URL: [Your Render URL will appear here after deployment]

## API Endpoints

### Transactions
- GET `/api/transactions` - Get all transactions
- POST `/api/transactions` - Create a transaction
- PUT `/api/transactions/:id` - Update a transaction
- DELETE `/api/transactions/:id` - Delete a transaction

### Categories
- GET `/api/categories` - Get all categories
- POST `/api/categories` - Create a category
- PUT `/api/categories/:id` - Update a category
- DELETE `/api/categories/:id` - Delete a category

### Budgets
- GET `/api/budgets` - Get all budgets
- POST `/api/budgets` - Create a budget
- PUT `/api/budgets/:id` - Update a budget
- DELETE `/api/budgets/:id` - Delete a budget

## Deployment Steps

1. Create a [Render](https://render.com) account
2. Fork or clone this repository to your GitHub account
3. In Render:
   - Click "New +" and select "Web Service"
   - Connect your GitHub repository
   - Name: budget-tracker-api
   - Environment: Node
   - Build Command: `npm install`
   - Start Command: `node server/server.js`
   - Add Environment Variables:
     - `MONGODB_URI`: [Your MongoDB connection string]
     - `NODE_ENV`: production

## Local Development

1. Clone the repository
2. Install dependencies: `npm install`
3. Create `.env` file with:
   ```
   MONGODB_URI=your_mongodb_connection_string
   PORT=5000
   ```
4. Run: `npm run dev`

## Tech Stack
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- CORS 