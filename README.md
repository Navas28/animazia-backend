# ⚙️ Animazia - Backend API


The robust RESTful API powering the Animazia wildlife platform. Built with Node.js and Express, it handles everything from ticket bookings to secure payment processing via Stripe.

## 🚀 Features

- **📂 Modular Architecture:** Clean and organized route structure for better maintainability.
- **🗄️ MongoDB Integration:** Uses Mongoose ODM for efficient data modeling of animals, blogs, and bookings.
- **💳 Secure Payments:** Full Stripe integration for handling ticket purchases and donations.
- **📤 File Management:** Multer integration for handling image uploads for blogs and animal records.
- **📧 Communication:** Services for contact forms and newsletter subscriptions.
- **🛡️ Security:**
  - CORS enabled for secure cross-origin requests.
  - Environment variable protection via `dotenv`.

## 🛠️ Tech Stack

- **Runtime:** [Node.js](https://nodejs.org/)
- **Framework:** [Express.js](https://expressjs.com/)
- **Database:** [MongoDB](https://www.mongodb.com/) with [Mongoose](https://mongoosejs.com/)
- **Payments:** [Stripe API](https://stripe.com/docs/api)
- **Middleware:** [Cors](https://www.npmjs.com/package/cors), [Multer](https://www.npmjs.com/package/multer), [Body-parser](https://www.npmjs.com/package/body-parser)
- **Utilities:** [Dotenv](https://www.npmjs.com/package/dotenv), [Nodemon](https://nodemon.io/) (Dev)

## 📡 API Endpoints (Overview)

| Endpoint          | Description                                  |
| :---------------- | :------------------------------------------- |
| `/animals`        | Manage species information and Red List data |
| `/ticketbooking`  | Handle zoo visit bookings                    |
| `/blogs`          | Eco Journal content management               |
| `/donate`         | Process conservation donations (Stripe)      |
| `/event-register` | Handle registrations for zoo events          |
| `/job-apply`      | Manage volunteer and job applications        |
| `/contact`        | Process contact form submissions             |
| `/subscribe`      | Email newsletter management                  |


## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)
- MongoDB Atlas account or local installation

### Installation

1. **Navigate to backend folder:**

   ```bash
   cd backend-animazia
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Environment Setup:**
   Create a `.env` file and configure the following:

   ```env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   STRIPE_SECRET_KEY=your_stripe_secret_key
   ALLOWED_ORIGINS=http://localhost:5173
   ```

4. **Start the server:**

   ```bash
   # Development mode
   npm run start

   # Production mode
   node index.js
   ```

---

