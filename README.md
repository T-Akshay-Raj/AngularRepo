# AngularRepo
Angular Practice Repo


# Angular

## Prerequisite Softwares
- Node.js(check version using :  node -v)
- NPM(check version using :  npm -v)
- IDE: VS Code(Recommended) 

>Note: node.js can be downloaded from [nodejs](https://nodejs.org) and VS code from [vscode](code.visualstudio.com)

## Prerequisite technical knowledge
- HTML
- CSS/SCSS
- TypeScript/Java Script

> Angular official Documentation at [Angular docs](https://angular.io/docs)

## Angular CLI
- Install Angular cli
    - npm install -g @angular/cli  (Installs latest version)
    - npm install -g @angular/cli @11 (Installs specific version)




## Angular commands:
Angular's command line tool is called ng

## Create Sample dryrun angular project
ng new app-name --dry-run
- All other ways to generate a new application can be found using help
    -   ng new --help
 
> Note: After creating the project, you may open it directly in vs code using below steps, First navigate to workspace folder where app is created and in cmd enter 'code .'

# Project Structure
- source folder
  - app folder
  - main.ts file

- Package.json - holds project description and its dependency information(similar to pom.xml)
- angular.json - contains config information used by cli for various angular phases(like build, serve, test, lint)
- karma.conf.js - used by cli for test related information
- tsconfig.json - contains compiler options
- tsconfig.app.json - contains compiler options for application code
- tsconfig.spec.json - contains compiler options for test code 
- e2e folder:
  - protractor.conf.js - contains compiler options for test files
- environments folder - contains environment specific files

## Core Building Block of Angular

### Decorators
- Decorators are functions that returns functions
- They convey angular on code functionality and how to inject code
- Marked using '@' symbol
- Invoked during runtime with arguments
- Example decorators:
  - @NgModule() for modules
  - @Component() for components
  - @Injectable() for services
  - @Pipe() for pipes
  - @Directive() for directives
  - @Input for data flowing into a component
  - @Output for data flowing out of a component


## Run angular application
- command: 'ng serve'
- creates a local dev environment for the application, [local host url]("http://localhost:4200")
- Tip to run and open in browser: 'ng serve --open'

> For ng server options list, 'ng serve --help'

### Create files using schematics(ng generate)
- Get list of schematics and options available using 'ng generate --help'
- example schematics are (application, class, component, module, library, enum, module, interface, service etc)
- Example to generate component: 'ng generate component component-name' or 'ng generate component component-name --dry-run' or 'ng g c component-name --dry-run' (It creates 4 files : .ts, .html, .scss and .spec.ts file)
- Example to generate module : 'ng generate module module-name'. It generates a module and .ts file in it)

## popular angular commands
- ng: list all available commands
- ng new(alias n): Creates a new workspace and an initial angular app
- ng add: Adds support for an external library to your project
- ng build (alias b): compile code and output files into build directory
- ng serve(alias s): compile code and launch and dev server and watch the changes(means changes get auto reload instead of refresing window each time)
- ng generate(alias g): to add new files using angulars builtin boilerplates(for all options "ng generate --help")
- ng lint(alias l): runs angular lint
- ng test(alias t): run unit test in a project
- ng run: Runs an architect target with an optional custom binder configuration defined in your project
- ng help: to get help on angular commands
- ng --version(alias v): to check angular cli version
- ng e2e(alias e): run intergation tests
- ng update: updates application and its dependencies


## Additional helpful Plugins or tools
- Angular Language service(available as plugin in vs code by angular.dev)
- Angular dev tools: a browser extension which gives detailed debugging information in realtime when working with browser
- Angular scematics: Custom code collection, reusable across multiple projects


## Commands
### Test
Run Unit test(Auto run again on changes to tests): ng test
Run Unit Test(Without re run Doesn't auto run on change): ng test --no-watch
Code Coverage: ng test --code-coverage



- Jasmine: Testing Framework


# Update Angular version
- Verify assisted changes between from version and to version using [Angular Update](https://update.angular.com)
- Always suggested to perform incremental upgrade

### Quiz
1. What is the main benefit of using Angular over other modern JavaScript frameworks?

- Angular's ecosystem of tools that work together like a unified platform
- Angular's ecosystem of tools for building complex user interfaces
- Angular's ecosystem of tools that maximize compatibility with other libraries and frameworks

Answer: Angular's ecosystem of tools that work together like a unified platform

2. When does Angular release a new major version of the CLI tool?

- Every six months, on its own schedule
- when they release a new MAJOR version of the Framework itself
- As needed, independent of the Framework

Answer: when they release a new MAJOR version of the Framework itself

3. What's the best way to manage breaking changes in your code during a major version upgrade?

- Upgrade dependencies one at a time.
- Follow the recommended upgrade path.
- Upgrade all dependencies at the same time.

Answer: Follow the recommended upgrade path.

4. When might you want to avoid software released under the MIT License?

- when you want the copyright holders to be held liable if something goes wrong
- when you need a license compatible with the GNU General Public License
- when you want to release your own commercial software under a different license

Answer: when you want the copyright holders to be held liable if something goes wrong


5. What made Angular unique when it was first released back in 2010?

- strong community support after its release
- using Javascript to generate html at runtime
- its focus on extending HTML markup with custom attributes

Answer: its focus on extending HTML markup with custom attributes
