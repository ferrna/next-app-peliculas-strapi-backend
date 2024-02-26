# Initiate app in local environment
1. cd next-strapi-app-peliculas (NEXT Client) 
2. npm install 
3. npm run dev (to start the client in development) 

# cd ..
# cd next-app-pel-backend/next-strapi-app-peliculas (STRAPI Server)
4. For using Strapi its needed an even version of node.js (example ^18.19.0) [If you are using Windows you can install a node version using nvm 'nvm list available; nvm install 18.19.0; nvm use 18.19.0 (to use the new version 18.19.0 in current path folder, or 'nvm alias default 18.19.0' to select the new version as the default)'] 
5. Then run npm install in cd next-app-pel-backend/next-strapi-app-peliculas and modify the env files with the next values with your cloudinary cloud-name (create one if don't have one): 
```
CLOUDINARY_NAME=""
CLOUDINARY_KEY=""
CLOUDINARY_SECRET=""
```
6. Then use npm run develop to start the server, and that's all 
```
Next client will be running in localhost:3000
Strapi backend will be running in localhost:1337
```
```
You can test calling localhost:1337/api/peliculas?filters[enlaceUrl][$eq]=the-terminator , to get the data for The terminator movie i.e. or 
localhost:1337/api/peliculas?populate=* to get all the movies in the Strapi database with images and relations 
```

# 🚀 Getting started with Strapi

Strapi comes with a full featured [Command Line Interface](https://docs.strapi.io/dev-docs/cli) (CLI) which lets you scaffold and manage your project in seconds.

### `develop`

Start your Strapi application with autoReload enabled. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-develop)

```
npm run develop
# or
yarn develop
```

### `start`

Start your Strapi application with autoReload disabled. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-start)

```
npm run start
# or
yarn start
```

### `build`

Build your admin panel. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-build)

```
npm run build
# or
yarn build
```

## ⚙️ Deployment

Strapi gives you many possible deployment options for your project including [Strapi Cloud](https://cloud.strapi.io). Browse the [deployment section of the documentation](https://docs.strapi.io/dev-docs/deployment) to find the best solution for your use case.

## 📚 Learn more

- [Resource center](https://strapi.io/resource-center) - Strapi resource center.
- [Strapi documentation](https://docs.strapi.io) - Official Strapi documentation.
- [Strapi tutorials](https://strapi.io/tutorials) - List of tutorials made by the core team and the community.
- [Strapi blog](https://strapi.io/blog) - Official Strapi blog containing articles made by the Strapi team and the community.
- [Changelog](https://strapi.io/changelog) - Find out about the Strapi product updates, new features and general improvements.

Feel free to check out the [Strapi GitHub repository](https://github.com/strapi/strapi). Your feedback and contributions are welcome!

## ✨ Community

- [Discord](https://discord.strapi.io) - Come chat with the Strapi community including the core team.
- [Forum](https://forum.strapi.io/) - Place to discuss, ask questions and find answers, show your Strapi project and get feedback or just talk with other Community members.
- [Awesome Strapi](https://github.com/strapi/awesome-strapi) - A curated list of awesome things related to Strapi.

---

<sub>🤫 Psst! [Strapi is hiring](https://strapi.io/careers).</sub>
