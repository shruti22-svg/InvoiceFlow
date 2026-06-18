# InvoiceFlow
A MERN stack invoicing application for freelancers and small businesses.

## 🔴 Live Demo
👉 https://invoice-flow-ybn5.vercel.app

## Features
- Send invoices, receipts, estimates and quotations via email
- Download invoices as PDF
- Set due dates and track payment status
- Record full and partial payments with payment history
- Dashboard with invoice statistics
- Google authentication and JWT support
- Multiple user registration

## Tech Stack
**Client:** React, Redux, Material UI, Axios, Apex Charts

**Server:** Node.js, Express, Mongoose, JWT, Nodemailer

**Database:** MongoDB Atlas

## Setup

Split your terminal into two — one for client, one for server.

**Client**
```bash
cd client
npm install
npm start
```
Create `client/.env`:
REACT_APP_GOOGLE_CLIENT_ID =

REACT_APP_API = http://localhost:5000

REACT_APP_URL = http://localhost:3000

**Server**
```bash
cd server
npm install
npm start
```
Create `server/.env`:
DB_URL =

PORT = 5000

SECRET =

SMTP_HOST =

SMTP_PORT =

SMTP_USER =

SMTP_PASS =

## Docker
Add `.env` files as above then run:
```bash
docker-compose -f docker-compose.prod.yml build
docker-compose -f docker-compose.prod.yml up
```

## Troubleshooting
PDF not working? Run:
```bash
npm install html-pdf -g
npm link html-pdf
npm link phantomjs-prebuilt
```

## Author
[@shruti22-svg](https://github.com/shruti22-svg)

## License
MIT