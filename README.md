# TestApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.2.16.
The V16 angular template project was upgraded to Angular V17.x.

Purpose: Evaluation of Angular CLI Migration Issue 29661 
https://github.com/angular/angular-cli/issues/29661#issuecomment-2688197220

Executing the following migration update, or upgrading to Angular V18 + apply the application builder migration
CLI >> ng update @angular/cli --name use-application-builder

Results in:
✖ Migration failed: Path "tsconfig.server.json" does not exist.

Background:
The angular.json "server" settings were originally defined within the default 'Visual Studio Angular Full-stack Template' from 2021
This template used V8 of angular, and over the years was upgraded to Angular V18 today.  The original "server" settings were never used, or changed as per Repo.


Error log:
[error] Error: Path "tsconfig.server.json" does not exist.
    at HostTree.readText (C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@angular-devkit\schematics\src\tree\host-tree.js:220:19)
    at new JSONFile (C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@schematics\angular\utility\json-file.js:23:34)
    at updateBuildTarget (C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@schematics\angular\migrations\use-application-builder\migration.js:83:28)
    at updateBuildTarget.next (<anonymous>)
    at C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@schematics\angular\migrations\use-application-builder\migration.js:129:19
    at C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@schematics\angular\utility\workspace.js:64:30
    at async callRuleAsync (C:\Users\[user]\AppData\Local\Temp\angular-cli-packages-enN7Z7\node_modules\@angular-devkit\schematics\src\rules\call.js:80:18)





## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
