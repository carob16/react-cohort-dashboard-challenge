## Instructions

[Implement this design](./_assets/dashboard.png) using, as a minimum, the below listed technologies. Note: you may need to open the file directly on your machine to view it properly.

- ReactJS
- React Router DOM version 6.4 or above (Run `npm install react-router-dom` to install this)
- A RESTful API

[Use this REST API](https://boolean-api-server.fly.dev/api-docs/#/post) as your data source. Use the **post** endpoints, which contains routes for posts and comments. Each of these routes has GET, POST, PUT and DELETE methods available. Post and comment authors are linked to the contacts retrieved from the **contact** endpoints via a `contactId` property, which will allow you to retrieve information about post and comment authors.

## Core Requirements

- Everything that *can* be its own component, *should* be its own component. You **must** provide evidence of planning what components you are going to create - this could be a component tree diagram, a bullet point list, a wireframe, whatever you like. Include your plan as a file in this repository.
- Users should be able to create a new post. The new post should be displayed at the top of the post feed.
- Users should be able to comment on existing posts.
- Posts and comments should show the initials of the author in a coloured circle.
- Clicking a posts title (under the author name) should take the user to a separate route that shows only that post and all of its comments. You **must** use a route for this, not an array filter.
- You must use [this style guide](./STYLE_GUIDE.md) to implement the colour scheme.
- The layout does not need to be mobile responsive, nor does it need to be pixel perfect. Get as close as you can, but your main focus should be on React - not CSS.

## Extension Requirements

- Use the Context API to reduce prop drilling of state
- Only 3 comments should be visible on a post; if a post has more than 3 comments, the `See previous comments` link should expand the list of comments to display all of them. => create variable toggle when clicked. If()=> pass in all or 3 comments
- Clicking on a post / comment authors name or initials, the user initials in the top right of the app, or the `Profile` link in the left navigation menu should take the user to [this Profile screen](./_assets/profile.png).
    - Use the contact with an ID of 1 to emulate the currently logged in user. This is the user you should use when clicking the top right initials or the Profile menu item directly.
    - The fields should be automatically populated with the correct data when loading any user profile.
    - Note that the design provided only shows example form fields to demonstrate roughly how the design of the page should look, you should inspect what data is available on a Contact entity to decide which fields you'll actually create.
- You should be able to update all of the users information.
- Posts and comments should be able to be updated and deleted.

## Advice

Break this project down into smaller, individual tasks. You could use a simple todo list, a project management board like Trello, anything you like. Not only will this reduce overwhelm and provide you with a clear path forward, it'll also ensure you have understood and accounted for every requirement.
