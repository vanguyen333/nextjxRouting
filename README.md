This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

This is the template of creating nav bar nextjs routing
NOde version:18.17.1

# Questions to remember

1. Explain how does the Next.js routing differe from React.js routing?

a) React Routing,
-import all neessary packages from react-router-dom, we initialize our app
,which is a function component, wrap everything in a Router,Routes,
then we create new Route with a path and element for each of the pages we want to have within our application
import { BrowserRouter as Router, Route, Link, Routes} from 'react-router-dom';

const App = ()=>{
<Router>
<Routes>
<Route path="/" element={<Home/>}/>
<Route path="/about" element={<About/>}/>
<Route path="/contact" element={<Contact/>}/>
</Routes>
</Router>

export default App;

b) Nextjs routing
use a file-based routing system.
Folders are used to define routes
Files are used to create UI for that route segment
For instance, to convert the previous React.js routing example into Next.js
, we only need to create 2 folders named about and contact. We'll create a special file associated with that route segment inside each folder, such as
page.js or page.jsx

2.  What is the purpose of route groups, and how can they be created in Next.js? 16:54
    They help organize routes into logical groups.
    We can crete a route group by enclosing the folder, by enclosing the folder name in parentheses.
3.  What is a dynamic route, and why should we create dynamic routes in web applications?

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
