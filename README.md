<h1 align="center"><b>STRAPI.IO from Scratch</b></h1>
<p align="center">
  <img src="https://raw.githubusercontent.com/jvlessa/Strapi.io/main/media/repo_logo.png" width="450">
</p>
<br/>

## THIS REPOSITORY MAIN'S GOAL
- Studuying a bit about this headless and open-sourced CMS;

## NOTES
- [Official Documentation](https://strapi.io/documentation/developer-docs/latest/getting-started/introduction.html)
- Strapi is a flexible, open-source <b>Headless CMS</b> that gives developers the freedom to choose their favorite tools and frameworks while also allowing editors to easily manage and distribute their content. By making the admin panel and API extensible through a plugin system, Strapi enables the world's largest companies to accelerate content delivery while building beautiful digital experiences;

- Name comes from: Strapi comes from the word Bootstrap, and helps Bootstrap your API;

## INSTALLATION AND RUNNING STRAPI.IO
- [Guide Video](https://www.youtube.com/watch?v=zd0_S_FPzKg&feature=youtu.be)

1. Install your package:
- <b>NPM:</b>
- [Install Node.JS and NPM here](https://strapi.io/documentation/developer-docs/latest/installation/cli.html#step-1-make-sure-requirements-are-met);
- Refresh NPM to last version (at the time that I'm writing this, Strapi.io dependencies only accepts NodeJs on theses versions: ">=10.16.0 <=14.x.x"):
``npm install npm@latest -g``

- <b>YARN:</b>
- [Install Yarn Package here](https://yarnpkg.com/en/)

2. Run your package command:
- <b>NPM:</b>
``npx create-strapi-app my-project --quickstart``
- <b>YARN:</b>
``yarn create strapi-app my-project --quickstart``

3. Possible errors:
- The official video of Strap.io does not show dependencies errors, so I had to do some stuff on my own:
- Enter the folder project and run:
``npm install`` OR ``yarn install``

- Wait for everything to update
``npm run-script build`` or ``yarn run-script build``
- Run Strapi.io
``npm start`` or ``yarn start``

4. To edit and create "Content-Types Builder"
- Run Strapi.io
``yarn develop``

# OTHER KIND OF INSTALLATIONS
- <b>Strapi.io with MongoDB on Ubuntu:</b> [Clicke here](https://strapi.io/documentation/developer-docs/latest/guides/databases.html#mongodb-installation)

## IMPORTANT LINKS
- [How to run a Strapi dev stack with Docker compose](https://strapi.io/blog/how-to-run-a-strapi-dev-stack-with-docker-compose)

## RUNNING
- Open your browser at: http://localhost:1337/admin/;
- Create your ADMIN account;
- For default, the project is using a SQL Database;

## CREATING CONTENT TYPES
1. Click on "Content-Types Build" on the "Plugins" tab;
2. Click on "Create new collection type", for example: "ViewDeck";
3. Close the popup and create some fields;
4. Click on "Add another field";
5. For this example, I have created these fields:
- name: text
- description: rich text
- pictures: image
- user: relation with User Permissions;

## CREATING COMPONENT
1. Click on "Create new component";
2. When creating the Component, it asked me the category. I choose: "Page";
3. I have followed the documentation and created two components: "Gallery" and "Text-Block";
4. Created 2 fields for each component and saved;

## CREATING SINGLE TYPE
1. Click on "Create new Single Type";
2. Created one called "Homepage";
3. Added one text field called "title";
4. Then... I added a "Dynamic Zone" and picked the 2 components that I have created before it;

## ADDING CONTENT TO REPRODUCE
1. Add data to the Collections Types;
2. Add data to the Single Types using the components;

## SETTING ROLES AND PERMISSIONS
1. Go to the "Roles and Permissions";
2. Go to the "Public": http://localhost:1337/admin/settings/users-permissions/roles;
3. Allow those permissions:
- Application: find;
- [Our content-type name]: find, findone;

## PUBLISH
- If you do not click "Publish" on "ViewDeck's Content-Type" and "Homepage's Single-Type", they won't appear at the browser and API's;

## CONSUME THE API:
- Access the links: 
1. http://localhost:1337/view-decks
2. http://localhost:1337/homepage

- You should see the JSON files;

## PLUGINS
### Swagger
- To install and use it, go to "MarketPlace": http://localhost:1337/admin/marketplace;
- Search for "Documentation";
- Install it as an Administrator;
- Restart Strapi.io;
- Open "Extensions";
- Open "Documentations";
- Click "Open the documentation";

## HOW TO CONSUME THE CONTENT TYPE'S API
- Check [these documentations](https://strapi.io/documentation/developer-docs/latest/getting-started/quick-start.html#_9-consume-the-content-type-s-api) for the language or framework of your preference;
