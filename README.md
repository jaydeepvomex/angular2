# Angular 2

Performance - faster than Angular 2
Mobile support - creating SPA that works on mobile and desktop devices
Component based development - everything is component based, forms a building blocks of an Angular application

### More language choices
1. ECMAScript 5
2. ECMAScript 6 (also called ES2015)
3. TypeScript (most popular language) - has great support of ECMAScript 6 standard
4. Dart
5. PureScript
6. Elm

#### TypeScript
1. Free and open-source programming language developed by Microsoft
2. Superset of JavaScript
3. Transpilation compiles TypeScript to JavaScript

- TypeScript benefits
1. Intellisense
2. Autocompletion
3. Code navigation
4. Advanced refactoring
5. Strong Typing
6. Supports ES2015 (ES6) features like classes, interfaces and inheritance

- TypeScript is also supported by several code editors
1. Visual Studio
2. Visual Studio Code
3. Eclipse
4. WebStorm
5. Atom
6 Sublime Text etc.

## Installation
1. Node and NPM

2. In Visual Studio > Tools > Options > Projects and Solutions > External Web Tools
> Move the $(PATH) to 2nd position 

3. Install TypeScript for Visual Studio 2017
> Install from https://www.microsoft.com/en-us/download/details.aspx?id=55258

4. Create an Empty ASP>NET Web Application project
> File > New ASP.net Web Application project > Select Empty from ASP.net template and click OK

5. Download "Quick Start Files" from Angular website
> https:// github/angular/quickstart
> Download Zip folder and copy the required "Starter files" to the web applicaiton project

## Run the application

```bash
$ npm start
```

> The app loads the app.component.ts file 

``` javascript
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `<h1>Hello {{name}}</h1>`,
})
export class AppComponent  { name = 'Angular'; }
```

### Angular 2 Components

A component in Angular is a class with template and a decorator
- Template
- Class
- Decorator

1. Template defines the user interface, Contains the HTML, directives and data bindings
2. Class contains the code required for the template
3. Decorator adds the meta data to the class making it an Angular component

An example of a component
``` javascript
import { Component } from '@angular/core'

@Component({
    selector: 'my-employee',
    templateUrl: `app/employee/employee.component.html`,
    styleUrls: ['app/employee/employee.component.css']
})

export class EmployeeComponent {
    firstName: string = 'Tom';
    lastName: string = 'Hopkins';
    gender: string = 'Male';
    age: number = 20;
}
```