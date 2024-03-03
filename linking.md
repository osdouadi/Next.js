- What is the difference between linking and navigating ?
The difference is linking is when we use element responsible for linking such as the <a> or <Link /> in next js, and Navigating is when we use button for example to navigate.
The <Link /> Component is used in place of a in HTML and they are used for linking.
- Navigating.
For navigating we use <button> with onClick event, therefore we need to create a function for handling the navigation.
We need to import useRouter from next/navigation

"use client"
import {useRouter} from "next/navigation"
const page = () => {
const router = useRouter()
const openHome = () => {
router.push("/")
}
}

"use client"is used here because we are running it on the client side, remember whenever we are using client side fionctionalities in next.js we have to declare that by adding "use client" in the top level before our import statments.
- How to set active page?

import {usePathname} from "next/navigation"

const navbar = () => {

 const path = usePathname()
 const navLink = [
{
name: 'Home',
link: '/'
},
{
name: 'Services',
link: '/services'
},
{
name: 'About',
link: '/about'
}
 ]

}
<ul>
{
navLink.map((link) => {
const isActive = path === link.href
return (
<li className={isActive ? "nav-link active " : "nav-link"}>
<Link href={link.href}>
{link.home}
</Link>
</li>
})
}
</ul>

We create an array let's call it navlink, and in this array we use object with two properties let's call them name and link, the value of name is the name of the link and the value of the link is the href.
We also import usePathname from next/navigation
We create a condition const isActive = path === link.href. 
isActive is true whenever path is equal to link.href.


