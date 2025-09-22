


# AI Amazona Ecommerce

## About This App

AI Amazona Ecommerce is a modern, full-stack e-commerce platform inspired by Amazon, designed for learning, prototyping, and real-world online retail. It combines robust backend logic, a scalable database, and a beautiful, responsive frontend to deliver a seamless shopping experience for users and powerful management tools for administrators.

### Key Features

- **Storefront**: Users can browse products, view details, add items to their cart, and complete purchases with a secure checkout flow.
- **Authentication**: Secure login and registration using NextAuth.js, supporting multiple providers.
- **Shopping Cart**: Persistent cart state, cart badge, and intuitive add/remove functionality.
- **Order Management**: Users can place orders, view order history, and track order status. Admins can view all orders, update statuses, and analyze sales.
- **Admin Dashboard**: Metrics, revenue charts, recent orders, and product/category management for store owners.
- **Profile & Address Book**: Users can manage their profile and shipping addresses for faster checkout.
- **Payment Integration**: Ready for integration with Stripe or other payment gateways for real transactions.
- **Product Catalog**: Dynamic product listing, filtering by category, and related product suggestions.
- **Reviews & Ratings**: Users can leave reviews and ratings for products.
- **Mobile-First UI**: Responsive design using Tailwind CSS for optimal experience on all devices.

### Architecture

- **Frontend**: Built with Next.js (App Router), React, and TypeScript for fast, maintainable code.
- **Backend**: Next.js API routes handle authentication, product, order, and payment logic.
- **Database**: PostgreSQL managed via Prisma ORM, with migrations and seed data for easy setup.
- **State Management**: React context and custom hooks for cart and session state.
- **Reusable Components**: Modular UI components for forms, tables, dialogs, and more.

This project is ideal for:
- Developers learning full-stack web development
- Building MVPs for e-commerce startups
- Experimenting with modern web technologies
- Customizing for real-world online stores

Visit the deployed app here: [https://ai-amazona-ecommerce.vercel.app/](https://ai-amazona-ecommerce.vercel.app/)


## Getting Started

### Prerequisites
- Node.js >= 18.x
- PostgreSQL database

### Installation

```bash
# Clone the repository
git clone https://github.com/snjugunanjenga/ai-amazona-ecommerce.git
cd ai-amazona-ecommerce

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your database and auth credentials

# Run Prisma migrations and seed data
npx prisma migrate dev
npx prisma db seed

# Start the development server
npm run dev
```

### Database Setup
- Update `prisma/schema.prisma` for your DB config
- Use `npx prisma studio` to view/manage data

## Usage
- Visit `http://localhost:3000` for the storefront
- `/admin` for admin dashboard
- `/dashboard` for user dashboard

## Scripts
- `npm run dev` — Start development server
- `npm run build` — Build for production
- `npm run lint` — Run ESLint
- `npx prisma migrate dev` — Run DB migrations
- `npx prisma db seed` — Seed database

## Contributing

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/foo`)
3. Commit your changes (`git commit -am 'Add feature'`)
4. Push to the branch (`git push origin feature/foo`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgements
- [Next.js](https://nextjs.org/)
- [Prisma](https://www.prisma.io/)
- [Tailwind CSS](https://tailwindcss.com/)
- [NextAuth.js](https://next-auth.js.org/)
- [Stripe](https://stripe.com/) (for payment integration)

---

For questions or support, please open an issue or contact the maintainer.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
