# End-Goal
To create a single-page MERN stack application to solve a real-world problem.

# Goals for Day 1
- [ ] boilerplate set up for repository
- [ ] models created
- [ ] typedefs for each model
- [ ] create queries and resolvers and test in the playground

# Main Points to Remember
- `React` front end
- `GraphQL API` with `NodeJS` and `Express.js` server
- Use `Queries` and `Mutations` for CRUD interactions with data
- Authentication with `JWT`
- Deployed on `Heroku`
- Polished UI
- Mobile-responsive
- Protect API keys and other sensitive variables
- Clean, well-organized repository using best-practices for naming, structure, etc.
- High-quality README with screenshots and link to deployed app

--------------------------

# How to Initially Set Up the Repo
- create a repository on Github and set permissions to protect the main branch (refer to `06-Server-Side-APIs/01-Activities/25-Stu_Git-Repo-Setup` if you need a refresher on how to do this)
- initialize the repository as `Node` application - (run `npm init -y`)
- run `npx create-react-app client` to create the `client` folder in the root level of the repository
- create a `server` folder in the root level of the repository
- create internal folder structure in `server` (refer to `Unit 21 mini-project` for what folders and files will be needed)

# Things to Plan (for Server)
- what `Models` do I need in my application?
- need to set up `connection.js` to connect to MongoDB 
- `typeDefs.js` - for each `Model`, we need a type definition. What data should be returned when my `Model` is queried? what entrypoints do I have to access data (`queries`)? how can my data be updated (`mutations`)?
- `resolvers.js` - for each `Query` and `Mutation`, we need to write the actual functionality to make the `typeDefs` work.
- `server.js` - connect to ApolloServer, setup Express app, etc. (Refer to `Unit 21 mini-project` for a good example of how to setup server)
- `utils` folder - need to setup authorization via `JWT`. Any sort of backend helper functions would go here too (format date functionality maybe?)

# Things to Plan (for Client)
- what `Components` and `Pages` do I need for my front end React app?
- `utils` folder - need to define the `mutations` and `queries` here. Also, any other front end helper functions. (Refer to `Unit 21 mini-project` for good examples)
- What is the heirarchy for my App? How am I passing data from one component to another?
- `useState` hooks - (refer to `20-React/01-Activities/11-Ins_State` for how to set up `useState`)
- `useEffect` hooks - (refer to `20-React/01-Activities/17-Ins_Hooks-useEffect` for how to set up `useEffect`)



### Resources
- [How to Map Data into Components in React](https://www.geeksforgeeks.org/how-to-map-data-into-components-using-reactjs/)