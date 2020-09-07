# Postgres Explain Visualizer (pev)

Postgres Explain Visualizer (dev) is designed to make [EXPLAIN](http://www.postgresql.org/docs/current/static/sql-explain.html) output easier to grok. It creates a graphical representation of the plan. You can see it in action at [tatiyants.com/pev](http://tatiyants.com/pev/), or read about it [on my blog](http://tatiyants.com/postgres-query-plan-visualization/).

Pev is heavily influenced by the excellent [explain.depesz.com](http://explain.depesz.com/).

Pev is written in [angular 2](https://angular.io/) with [TypeScript](http://www.typescriptlang.org/). The project is based on [angular2 seed](https://github.com/mgechev/angular2-seed). It requires [npm](https://www.npmjs.com/), [gulp](http://gulpjs.com/), [tsd](http://definitelytyped.org/tsd/), and [compass](http://compass-style.org/).


## Installation

```
npm install
npm start
```

You may also need to install tsd and compass:

```
npm install tsd -g
gem install compass
```

## Build
To build, run the build command for a specific environment. For example, the following will create a production distribution:

```
npm start build.prod
```

## Updates (2020)

rm -rf node_modules
nvm install 4.0.0
npm -v

- config.ts:
export const VERSION_NPM = '2.14.7';
export const VERSION_NODE = '4.0.0';

- remove from package.json

   "karma-phantomjs2-launcher": "^0.3.2",

```bash
git remote remove origin
git remote add origin git@github.com:ilovejs/pev3.git
git branch --set-upstream-to=origin/master master
git pull
git push origin master --force
```
