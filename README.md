# swe-sr-8-1

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt

![Fullstack Diagram](./client-server-database-diagram.svg)

You’ve been given a diagram (see above) showing the three core layers of a fullstack application:

- Frontend – a React application that users interact with
- Backend – an Express server that handles logic and communication
- Database – a PostgreSQL database that stores persistent data

Imagine you’re explaining how these layers work together by using a real-world example: Instagram.

Your task:

1. Explain how Instagram works using the three-layer diagram.

   - What happens when a user opens the app, scrolls through their feed, likes a post, or uploads a new photo?
   - Walk through how data flows from the frontend to the backend and to the database—and back again.

2. Come up with an analogy to help someone new to coding understand these layers.

- You might compare the system to something like a restaurant, a library, or even a post office—anything that helps make the roles of each layer intuitive.
- Make sure your analogy maps clearly to the roles of the frontend, backend, and database.

3. Reflect on the value of this separation.

- Why do we separate concerns into these layers?
- What would go wrong if we tried to do everything in one layer?

Audience: Imagine you're writing this for someone who's just starting out in web development and wants to understand how modern apps work.

Length: Around 400–600 words.

## Response

In regards to Instagram, when you go on the homepage, The frontpage is what is visible to you the user. The stories on the top, posts to scroll through under, and the various buttons (messages, like, comment, share). As soon as you do open the app a request is sent to the backend. The backend is a server and the front end is essentially saying "get me all of the posts for these users" This is processed in the backend and is sent to the database in the form of queries which fetch the data. In this case it fetches the posts from people you follow/know including the captions, likes, and comments. The server compiles this data and sends it back to the frontend and its rendered on your feed. When you upload a post, on the frontend its as simple as pressing share, this sends the post/information(data) to the backend to be processed, could be resized or check for errors, then its sent to the database where the meta data would be stored, things like the captions, user id, in some cases the actual post/image may be saved in a cloud service and the url to that would be saved in the database. then the backend sends a response to the frontend saying success and you post is now live and on your feed.

As far as an anology is concerned. I would think of it like a resturaunt. I prefer 5 star rating, even 3 michellen stars. The frontend is the waiter, its who you interact with on the surface level, you get your menu and order, much like interacting with a UI or Ordering something/creating a post. The backend is the kitchen. Everything is cooked back there, things are proccessed, cooked and gets things ready. Its exactly what a backend server is for. The kitchen doesnt store the food, and never saved its cooked and given to a waiter when its ready. Finally the Database is the pantry/the walk-in/storage. It stores all the ingredients (data). if a new dish is going to be prepared at the resturaunt, the kitchen will add new ingredients to the pantry, and when its time to cook they will retrive the ingredients, prep the food to its final product and serve it to the waiter where it will be presented to the user! To wrap it up nicely, you tell the waiter (frontend) what you want. They talk to the kitchen (backend), which pulls ingredients from the pantry (database), cooks your meal, and sends it back out to you!

We do this with the idea of seperation of concerns. To put it simply, things that relate and belong together should go together. This is done to keep our file structure organized and most importantly clean. If we were to just have all our files together, sure we might know whats going on as we're building it but what happens when you step away for a day or two. When you come back youre going to be confused for a while figuring out what files are what and this just isnt efficient. This way you make your life easier, and its better for scalability and flexibility!
