# nextjs-dashboard
Learning how to use Next.js with Dashboard Tutorial
=======
## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## What I've learned through this tutorial:

### 1. CSS Styling
- Using the `clsx` library to toggle class names based on state or other conditions.

### 2. Optimising Images
- The `<Image>` Component is an extension of the HTML `<img>` tag and has automatic image optimisation that prevents layout shifts when loading images.

### 3. Creating Layouts and Pages
- Using a file-system routing where folders are used to create nested routes.
- Create separate UI for each routes using `layout.tsx` and `page.tsx` files.
- The page is a React Component that allows the route to be accessible by the application.
- The layout file contains UI that can be shared between multiple pages.
- Partial rendering - only page components updates

### 4. Navigation
- Use the `<Link>` component to link between pages. Allows client-side navigation with JavaScript.
- Display an active link using the wthe `usePathName()` hook in Next.js.

### 5. Setting up the Database
- Create a Postgres database and linking it to the project on vercel.

### 6. Fetching data
- Fetching data using React Server Components.
- Use SQL query to fetch data (invoices).
- Parallel data fetching using `Promise.all()` or `Promise.allSettles()` to initiate all data requests at the same time to prevent request waterfalls

### 7. Streaming
- Streaming a page with `loading.tsx`. The page is split into parts that are rendered in parallel. 
This reduces the overall loading time and prevents slow data requests from blocking.
- Using loading skeletons - simplified UI as a placeholder to show the user the page content is loading.

### 8. Partial Prerendering 
- Use React's Suspense to defer rendering parts of the application until a condition is met (eg data is loaded).
- Adding `ppr` to next.config.mjs file.

### 9. Search and Pagination
- use Next.js APIs: `useSearchParams`, `usePathname`, and `useRouter`.
- Implement search and pagination with URL search parameters.

### 10. Mutating Data
- Use React Server Actions to mutate data.
- Working with forms and Server Components.
- Extracting, validating, and inserting data into the database.
- Revalidating and redirecting with `revalidatePath` from Next.js
- Updating and deleting invoices.

### 11. Handing Errors
- Use `error.tsx` to catch errors and show a fallback UI to users.
- How to use the `notFound` function and file to handle 404 errors (for resources that doesn't exist).
