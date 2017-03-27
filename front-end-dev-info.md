# Front-end Development

### [Hack OR Front-End Starter](https://github.com/hackoregon/hackoregon-frontend-starter)

This is a starter kit for Hack Oregon front-end development using React + Redux. This repo should help get started and keep the different projects aligned.
_____

### [Hack Oregon's React Component Library](https://github.com/hackoregon/component-library)

Hack Oregon's [React](https://facebook.github.io/react/) Component Library is a work in progress that encompasses platform components, a style guide, as well as data visualization components to be shared across projects.

For styling, we are using [CSS Modules](https://github.com/css-modules/css-modules).

The components that end up here are either built using [React Storybook](https://getstorybook.io/) or were ported into the Storybook dev environment. We believe this will allow us to make cross project compatible components.

Documentation for usage of these components and visual examples will be available on the [Hack Oregon's Storybook](https://hackoregon.github.io/component-library/?selectedKind=Welcome&selectedStory=to%20Storybook&full=0&down=1&left=1&panelRight=0&downPanel=kadirahq%2Fstorybook-addon-actions%2Factions-panel).

___

### Working with the component library and the project site at the same time

The component library is required by each project site using an npm dependency. Npm offers a utility called [`npm link`](https://docs.npmjs.com/cli/link) for using a local copy of a dependency when developing.

Once you have cloned both the component library and this project site, do the following:

1. `cd` to your local component-library checkout
2. Run `npm link`
3. `cd` to your local project site checkout
4. Run `npm link react-component-library`

Now any code in the project site that relies on components from the component library will import modules directly from your local checkout of component-library. Likewise, any changes you make to your local checkout of component-library will impact the project site. The project site will also watch these component-library changes and hot reload localhost:3000 for you.

___

### CIVIC Platform and project pages rendering

[CIVIC platform core](https://github.com/hackoregon/civic-platform)

[CIVIC Server](https://github.com/hackoregon/civic-server)

A server lib for server side rendering with examples of Civic App running 2 additional client side (project) apps
