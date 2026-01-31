# CampusTrade

> The trusted peer-to-peer marketplace for your campus community.

CampusTrade is a secure, real-time e-commerce platform built for university students. It allows students to buy, sell, and trade textbooks, furniture, and electronics within a verified network, ensuring safer transactions and local convenience.

## Tech Stack

*   **Framework:** Next.js 14+ (App Router)
*   **Styling:** Tailwind CSS
*   **Backend:** Supabase (PostgreSQL)
*   **Auth:** Supabase Auth
*   **Storage:** Supabase Storage (for images)
*   **Icons:** Lucide React

## Features

*   **Verified Community:** Authentication flow designed for university environments.
*   **Real-time Feed:** New listings pop up instantly via Supabase Realtime.
*   **Easy Selling:** Simple listing creation with image uploads.
*   **Dashboard:** Manage your active listings and mark items as sold.
*   **Search & Filter:** Quickly find textbooks or dorm essentials.

## Getting Started

1.  **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/campustrade.git
    cd campustrade
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Environment Setup**
    Create a `.env.local` file and add your Supabase credentials:
    ```bash
    NEXT_PUBLIC_SUPABASE_URL=your_url
    NEXT_PUBLIC_SUPABASE_ANON_KEY=your_key
    ```

4.  **Run the development server**
    ```bash
    npm run dev
    ```

## Documentation

*   [TASKLIST.md](./TASKLIST.md) - Tracking project progress.
*   [LEARNINGS.md](./LEARNINGS.md) - Technical decisions and lessons learned.
*   [.dev0/RULES.md](./.dev0/RULES.md) - Coding standards and AI guidelines.