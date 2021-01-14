<h1 align="center"><b>STRAPI.IO</b></h1>
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

## IMPORTANT LINKS
- [How to run a Strapi dev stack with Docker compose](https://strapi.io/blog/how-to-run-a-strapi-dev-stack-with-docker-compose)