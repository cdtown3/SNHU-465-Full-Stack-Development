# SNHU-465-Full-Stack-Development

# Architecture
In this project I utilized HTML & JS via Express and Angular as my frontend architectures. On my customer-facing side, I created HTML documents with JavaScript to display my data, which was served by Express. Using this MVC architecture, multiple pages were loaded one at a time as the user requested them. I used Angular on my admin-facing side, however, and I created multiple components that were loaded programatically within the same HTML document. They were preloaded, which provided for a seamless experience for admins to bounce around. Instead of loading and caching a new page, the code was already on the client waiting to be called. As for the backend, I utilized MongoDB, a NoSQL database that works extremely well with Node.JS. This database scales well and the fact that it stores documents in BSON means the conversion to JSON is generally painless.

# Functionality
In this project I used JSON as a way to store and display data. JSON is frequently used when sending data to or from a server, and it formats the data in user-friendly objects. JavaScript, on the other hand, is an extremely common language used by developers to manipulate the way their webpages behave. As mentioned above, MongoDB stores data in BSON format, which is binary JSON. We can then pull this via the MongoDB driver, and reformat the data to JSON. We can then use that data using Handlebars and TypeScript. In this way, JSON helps bridge between the backend and frontend.

I really enjoyed using Handlebars to display data programatically. It was very simple to use and I felt that it made for efficient code. Similarly, in Angular I was able to write an ngFor on a template, which allowed me to easily display all of the data in my query with minimal code. Along with this, Angular is extremely efficient in its use of components, in that if we have components that share the same component, we can use the child component like a template. This reusability is great to work with and keeps the code clean.

# Testing
Security is very important, which is why on the admin side we encrypted passwords and used hashes, rather than sending raw passwords to and from the database. It's also important to keep this hash off of platforms like GitHub. By creating interfaces for the database we can help prevent attacks like SQL Injection. We also must check the user or admin's permissions before allowing them to perform certain actions via the API. 

# Reflection
Full stack development can be tough to jump into with the tons of different frameworks and stacks you could use. This course was great because it forced me to stick on one stack throughout an entire project, and that dedication is what's needed to learn a library and framework. Due to this course I have a much better understanding of Node.JS, MongoDB, Express, and how they work together to create a flexible development environment.
