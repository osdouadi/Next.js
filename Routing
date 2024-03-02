- In next.js we have in-build routing, before version 12 of next.js we would have file based routing, but after v13, next.js is promoting app routing.
- Questions:
- What is file based routing system in next.js?
- How to create root in next.js?
- How folder is used as root in App routing in next.js?
- What is the use of page.js when it comes to Routing in next.js?
- Answers:
- What is file based routing system in next.js?
- By default we do not have to install any liberary for routing in next.js.
- Whenever we create a folder in the app folder that folder will be a root that can be used in the URL, this is why we say file based routing.
- If we create another folder inside the folder we created earlier this new folder will become a nested root.
- Example:
- Insead App folder we are going to create a new folder called Home.
- Home is a root now therefore we can type in the url: /Home
- Inside the folder that is called Home we created a new folder called Categories.
- Categories is a nested root: /Home/Categories.
- How folder is used as root in App routing in next.js?
- When we create a folder in the App Directory that folder will become a root.
- What is the use of page.js when it comes to Routing in next.js?
- the file page.js is used as a homepage in next.js app, therefore in the home directory that we created earlier we have to create a new folder called page.js, or page.jsx or page.tsx if you are using TypeScript.

const page = () => {
    return <div>Home Page</div>
}

export default page

 the page.jsx will automaticlly excute when you visit /home. because it is the entry point of that root. just like index.html, index.php or index.js..etc.


