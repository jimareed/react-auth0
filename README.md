# React Auth0

react single page app that uses auth0 for authentication.  

Config setup
1. create auth0 account
2. create app
3. set Allowed Callback URLs and Allowed Logout URLs and Allowed Web Origins to http://localhost:3000

Initial setup
```
npm install
npm install @auth0/auth0-react
```

Run
```
npm start
```
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Docker build
```
docker build --tag react-auth0-image .
docker run --name react-auth0 -it -p 3000:3000 -d react-auth0-image
```

Docker cleanup
```
docker rm -f react-auth0
docker rmi react-auth0-image
```

Production Build
```
  npm run build
  npm install -g serve
  serve -s build
```
