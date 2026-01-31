# Task List

This file shows the current progress of all tasks in this project.
It is automatically updated by dev0 as tasks are completed.

---

## Phase 1

- [ ] ⏳ **Project Scaffolding & Configuration**
  Initialize a new Next.js App Router project. Configure Tailwind CSS, install `lucide-react` for icons, and set up the basic folder structure (components, lib, app). Create a global layout with a responsive navbar and footer placeholder.

- [ ] ⏳ **Supabase Integration & Database Schema**
  Set up the Supabase client in the project. Define the SQL schema for `profiles` (linked to auth.users) and `items` (title, description, price, category, image_url, seller_id, created_at). Apply Row Level Security (RLS) policies to ensure users can only edit their own items.

- [ ] ⏳ **Authentication Implementation**
  Implement the Auth flow using Supabase Auth. Create a Login/Signup page. Implement middleware to protect private routes (like /create-listing). Ensure the auth flow properly creates a record in the `profiles` table upon sign-up.

## Phase 2

- [ ] ⏳ **Image Upload Component**
  Create a reusable Image Upload component that uploads files to Supabase Storage buckets. It should handle file selection, preview, upload progress, and return the public URL of the uploaded image.

- [ ] ⏳ **Create Listing Feature**
  Build the '/sell' page. Create a form using Server Actions to insert a new row into the `items` table. Integrate the Image Upload component. Validate inputs (price must be positive, title required). Redirect to the item detail page on success.

- [ ] ⏳ **Real-time Home Feed**
  Develop the main landing page displaying a grid of items. Implement Supabase Realtime subscription to listen for 'INSERT' events on the `items` table so new listings appear instantly at the top of the feed without a page reload.

- [ ] ⏳ **Item Detail Page**
  Create a dynamic route `/items/[id]` to display full details of a listing. Show the image, price, description, and seller info. Add a 'Contact Seller' button (mailto link or placeholder for now). Handle 404s if the item doesn't exist.

## Phase 3

- [ ] ⏳ **Search and Filter Logic**
  Add a search bar and category dropdown to the Home Feed. Update the database query to filter results based on text search (title/description) and category selection. Debounce the search input.

- [ ] ⏳ **User Dashboard**
  Create a `/dashboard` page where the logged-in user can see a list of items they are selling. Add 'Delete' and 'Mark as Sold' functionality using Server Actions.

## Phase 4

- [ ] ⏳ **UI Polish & Loading States**
  Implement Skeleton loaders for the feed and detail pages while data is fetching. Improve the styling of cards, buttons, and form inputs to match a cohesive 'campus' theme. Add toast notifications for success/error states.

## Phase 5

- [ ] ⏳ **Landing Page & SEO**
  Create a compelling hero section for non-logged-in users explaining the value prop. Add metadata (title, description, OpenGraph tags) to all pages for better sharing previews.

---

_Last updated by dev0 automation_
