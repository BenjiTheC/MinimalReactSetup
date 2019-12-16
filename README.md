# Minimal React development environment set up

I've been using [`create-react-app`](https://create-react-app.dev/) for React project initialization for a while. And I've been using [Material-UI](https://material-ui.com/) React components library for a while. Also, I've been using [`eslint`](https://eslint.org/) and [`prettier`](https://prettier.io/) for enforcement of coding style for a while.

The thing is, it's been kinda cumbersome for initial set up that before I can actually starting building something meaningful.

I will have to finish following steps before I can write the React component code:

1. Run `create-react-app` to initialize the project.
2. `npm install` and `npm install -D` dependency
3. Create `.eslintrc.json` and `.prettierrc` and make ESLint and Prettier work together properly. - This is annoying.
4. Delete unnecessary files such as `index.css`, `App.css` - I use JSS which is built into Material-UI and only _one_ tiny SCSS file for template HTML.
5. Create directories under `src/` - `assets/`, `components/`, `hooks/`, `pages/`. Potentially `redux/` and `services/`/`graphql/` if any state management or external API calls are needed, which is the case for 95% of the time.
6. Add customized fonts and theme in `assets/styles/`
7. Basic router(`'/'`) and context provider set up in `App.js`

Then I can finally write some components code.

So to simplify this workflow, I create this repo, to store pre-configured `package.json`, `.eslintrc.json` and `.prettierrc` for now. Eventually I will have a shell script (maybe python script) to do this for me.

