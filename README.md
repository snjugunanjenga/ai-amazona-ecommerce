

# AI Amazona Clone

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
