# software-engineer-pratice
A series of questions and a project to gage an engineer's skillset

# Part 1 - General questions

Try these without using a book or Google. If you need to, then use resources and make note of it.

- How can you secure your HTTP cookies against XSS attacks?
- What is agile development? What are the advantages of agile development?
- What is the difference between synchronous and asynchronous programming?
- How does the JavaScript event loop works?
- What is your understanding and experience with object-oriented programming (OOP)?
- What is your understanding and experience with functional programming?
- What does “non-blocking” mean in Node.js?


Consider the following JavaScript code:

```javascript
console.log("first");
setTimeout(function() {
    console.log("second");
}, 0);
console.log("third");
```
- Without running the code above, what do you think the output will be? Why? Now, run the code and check your answer. 

# Part 2 - CS coding problems

Limit yourself to 1 hour for each problem below. Try these without using a book or Google. If you need to, then use resources and make note of it.


1. Implement a function for fibonacci sequence
2. Given a sorted array, convert it into a binary tree
3. Explain the *time-complexity* of each of the problems above

# Part 3 - Small project: Veedeofy

I'd like you to build a small app to gage your current
skillset and ability in building software.

We'll call this app **Veedeofy**.

The idea is simple and fun since you'll get to work with Spotify and YouTube API.

[Spotify](http://www.spotify.com/), in case you haven't used it, is a music streaming app. 

You can download it on your iPhone or desktop and play with it.

On Spotify you can make playlists that are collections of songs.

Here's [one of my public playlists](https://open.spotify.com/user/sdvakili/playlist/6SMqwQ5NqWQGJX6ht2yNmM) of some Latin songs.

But, when we have a party it'd be nice to be able to play the video for each song. So, that's why we need to build Veedeofy.

Veedeofy takes a Spotify songs playlist and creates a YouTube video
playlist for each song. 

## Backend API services only

You don't need to build the front-end. But, as you plan/design the backend, it's important to consider the front-end and how the backend API service you build would work with a future front-end or mobile app. 


## Skills to demonstrate

- Use of Node with good practices, common middleware, etc.
- Ability to read and use 3rd party API documentation
- Ability to design and build a working solution
- The use of a database, like MySQL, MongoDB or Postgres
- The structure and organization of the Node app you build
- The organization and structure of your code
- The proper implementation of REST API patterns
- The use of patterns like: MVC, OOP, or Functional programming
- The use of a worker service that looks at the playlist table,
    this can be used to create the YouTube playlist based on the 
    Spotify playlist as a background job. And when the YouTube
    playlist is created the worker should update the main playlist
    table to save the YouTube playlist URL.

## Advanced mode (optional):

- Use of a few test cases and test-driven-development
- Deploy the app on AWS or Heroku for live access
- Use Redis for playlist conversion jobs


## Tips for success

- Make a plan of the things you need to build, along with sequence and schedule to help you complete the project
- Spend some time for researching the problem such as understanding the Spotify and YouTube APIs
- Track your time on each component of this project to know how long each part took for you to reasearch, design, and develop
- Use a paper or whiteboard to sketch the system architecture, database diagrams along with the components and sequence of events


### Example API
    CRUDL: Create Read Update Delete List Operations:
        http://localhost/api/v1/playlist

## Delivery
Create a GitHub repo and post your project there.

## Resources:
- [YouTube API](https://developers.google.com/youtube/v3/docs/)
- [Spotify API](https://developer.spotify.com/web-api/endpoint-reference/)
