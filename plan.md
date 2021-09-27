## PLAN

## models - Backend setup:

<!-- - Create a ElephantSQL DB and set up url in config.json -->
<!-- - Create a model for `space` -->
<!-- - Create a model for `story` -->

<!-- - Set up the relations migration (foreign keys => `userId` + `spaceId`) -->
<!-- - Set up relations in the models (hasMany, belongsTo, etc). -->

<!-- - Create some seeds for spaces and story. -->

<!-- - Try out some queries. findAll spaces, findByPk a space include stories, findByPk a user include his space -->

## Feature 1. List of spaces

Backend:

<!-- - Make a route that returns all the spaces. -->
<!-- - Try it out through httpie. -->

Frontend:

- Homepage is kinda set up.
- Fetch the data. => Thunk + axios and console.log the data.
- Setup a new slice (reduces) to store the spaces.
- Set up case and actions for this.
- Get data into redux and see it through the devTools.
- Set up a selector to get this data into my homepage
- Render it => set up a component like spaceCard that renders each space.

Space reducer:
Initial state =>
{ loading: true, allSpaces: [], details: {} || null }.

# COMMIT!

## Feature 2. Details of a space:

Backend:

- Create an express route that returns a specific space.
- GET - `spaces/:id`. router.get(`spaces/:id`, (req, res, next) => {...}) include the stories.
- Try it out with httpie, check im getting the space I want with the correct stories.

FrontEnd:

- Set up frontend route `/spaces/:id` and create a new page component for it.
- Set up a thunk to do the fetching.
- Have a place in redux to store this specific space.
- Get the space into redux => see devTools
- Selector and bring it to the page component
- Render it.
