Stripe Integration Project

A complete e-commerce demo with Next.js 15, Redux Toolkit, and Stripe Checkout.
Add products to cart, manage state globally, and securely checkout with Stripe.

Features

Works across the entire Next.js stack

App Router (Next.js 15) with API routes

Redux Toolkit for cart and global state

Stripe Checkout Session integration

Cart management: add, remove, update quantities

Success & cancel pages after checkout

Stripe Webhooks for payment confirmation

Styling with Tailwind CSS (default)

Demo

You can deploy this project on Vercel with your Stripe keys to get a live demo.

Deploy to Vercel

Vercel deployment flow will let you set up environment variables automatically.
Alternatively, you can clone this repo and run locally.

Clone and Run Locally

Clone repo:

git clone https://github.com/your-username/stripe-integration-project.git
cd stripe-integration-project


Install dependencies:

npm install


Rename .env.example to .env.local and add keys:

STRIPE_SECRET_KEY=sk_test_your_key
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=pk_test_your_key
NEXT_PUBLIC_APP_URL=http://localhost:3000
STRIPE_WEBHOOK_SECRET=whsec_your_key


Run the local server:

npm run dev


For webhook testing, use Stripe CLI:

stripe listen --forward-to localhost:3000/api/stripe/webhook

Feedback and Issues

Please file any issues or suggestions in the GitHub repository.
