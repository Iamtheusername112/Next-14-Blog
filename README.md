# Full-Stack Blogging Web Application

## Overview

This is a full-stack blogging web application built using modern web technologies. The front end is developed with Next.js, TailwindCSS, ShadCN UI, and TypeScript, while the backend and content management system (CMS) are powered by Sanity.io. The application is deployed on Vercel, and the Sanity.io backend is hosted on Sanity.

## Features

- **Real-time Content Management**: Utilize Sanity.io for dynamic content updates.
- **Responsive Design**: Styled with TailwindCSS for a mobile-first responsive design.
- **Rich Text Editing**: Use of PortableText for complex content structures.
- **Image Management**: Optimized image handling via Sanity.io.
- **Scalable Architecture**: Headless CMS approach for flexible frontend and backend integration.
- **Custom UI Components**: Developed with ShadCN UI for a tailored user experience.
- **TypeScript**: Ensures type safety and improved developer experience.

## Tech Stack

- **Frontend**: Next.js, TailwindCSS, ShadCN UI, TypeScript
- **Backend**: Sanity.io
- **Deployment**: Vercel (frontend), Sanity.io (backend)

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn
- Sanity CLI

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Iamtheusername112/Next-14-Blog.git
   cd your-repo-name
   ```

2. **Install Frontend Dependencies**

   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set Up Sanity.io Backend**

   - Install Sanity CLI globally:

     ```bash
     npm install -g @sanity/cli
     ```

   - Navigate to the `sanity` directory and initialize Sanity:

     ```bash
     cd sanity
     sanity init --create
     ```

   - Follow the prompts to set up your Sanity project and dataset.

4. **Set Up Environment Variables**

   Create a `.env.local` file in the root directory and add your environment variables:

   ```env
   NEXT_PUBLIC_SANITY_PROJECT_ID=your-sanity-project-id
   NEXT_PUBLIC_SANITY_DATASET=production
   NEXT_PUBLIC_SANITY_API_VERSION=2023-05-03
   ```

5. **Run the Development Server**

   ```bash
   npm run dev
   # or
   yarn dev
   ```

   Your application should now be running on [http://localhost:3000](http://localhost:3000).

## Deployment

### Frontend (Vercel)

1. **Connect Repository to Vercel**

   - Sign in to Vercel and create a new project.
   - Import your repository from GitHub, GitLab, or Bitbucket.
   - Follow the prompts to configure your project.

2. **Set Environment Variables**

   In your Vercel dashboard, go to the project settings and add the environment variables from your `.env.local` file.

3. **Deploy**

   Vercel will automatically deploy your project on push to the main branch.

### Backend (Sanity.io)

1. **Deploy Sanity Studio**

   From the `sanity` directory, run:

   ```bash
   sanity deploy
   ```

2. **Manage Content**

   Access your Sanity Studio at the deployed URL to manage your content.

## Project Structure

```plaintext
your-repo-name/
├── sanity/                   # Sanity.io project
│   ├── schemas/              # Sanity content schemas
│   ├── .sanityrc.json        # Sanity configuration file
│   ├── sanity.json           # Sanity project configuration
│   └── ...
├── src/                      # Next.js project source
│   ├── components/           # React components
│   ├── pages/                # Next.js pages
│   ├── styles/               # TailwindCSS styles
│   ├── lib/                  # Utility functions and sanity client
│   ├── types/                # TypeScript types
│   └── ...
├── public/                   # Public assets
├── .env.local                # Environment variables
├── next.config.js            # Next.js configuration
├── tailwind.config.js        # TailwindCSS configuration
├── tsconfig.json             # TypeScript configuration
├── package.json              # npm package configuration
└── ...
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License

This project is licensed under the MIT License.

## Contact

For any questions or feedback, please reach out to [iwufrancischisom20@gmail.com](mailto:iwufrancischisom20@gmail.com).

---
