[Home](../README.md)

# React Resources

Anything to do with React JS library 

Take a look at the [React Week Repo](https://github.com/foundersandcoders/react-week/blob/master/resources.md)

| Name          | Link          | What is it?  | Tip from
| ------------- | ------------- | ------------ | ------------ |
| Making setInterval Declarative with React Hooks | https://overreacted.io/making-setinterval-declarative-with-react-hooks/ | Good overview of potential pitfalls with useEffect | Oli
| RTL cheatsheet | https://testing-library.com/docs/react-testing-library/cheatsheet | React Testing Library Cheatsheet| Alex
| Article about React x Express  | https://daveceddia.com/create-react-app-express-backend/ | Learn how to connect a Create React App to an Express backend server | Reuben
| Tutorial - deploy React app + Express api server to Heroku | https://daveceddia.com/deploy-react-express-app-heroku/ | A step-by-step tutorial where you'll make a React app, an Express API server, and deploy both to Heroku | Reuben
| How to connect your React app to a backend on the same origin | https://flaviocopes.com/how-to-serve-react-from-same-origin/ | How to serve a React and a server-side backend app from the same origin, without having to use CORS on the server and worrying about ports |Reuben
| Proxying API Requests in Development | https://create-react-app.dev/docs/proxying-api-requests-in-development/ | Info from the react docs about proxying API requests in development | Reuben




### Slack note from Reuben re. the above React x Express articles:

hey all, something that everyone probably has questions about, I know I sure did after react week. how do I connect my react app to an express backend :open_mouth:

I’ve found a couple helpful articles for this, and theres a couple different ways of accomplishing this.

Just a quick refresher before you read though, create react app “bundles” all your react code into a folder called /build, and this is what netlify would serve, were you to deploy on netlify.

running the server on your machine, with npm start, i believe this process happens behind the scenes.

so these articles cover both running an express server and react app simultaneously on your local machine, and also in deployment, and if you come across “npm run build”, this is the step that netlify would do for you before it served your react app.

Also, for your student projects, React Router makes it much easier to have multiple pages in react, and some of these articles (or other articles on this subject) might mention it. 

It’s a slightly different concept to traditional routing that you’ve been doing in express, but not to worry, the docs are great, and im happy to answer any questions.

ok back to react+express. had some trouble finding articles written with hooks, but the component code isnt what we need here, and I tried to find articles that didnt just explain how to do it, but also how it works.

