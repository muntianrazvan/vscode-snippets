# vscode-snippets
Snippets I use on a daily basis. These snippets can come handy if you use Bootstrap, Font Awesome, Angular or Typescript.

## HTML Snippets
| Snippet     | Outcome                                                                   |
|-------------|---------------------------------------------------------------------------|
| ngclass     | `[ngClass]="{'${1:class}': ${2:condition}}"`                              |
| ngstyle     | `[ngStyle]="{'${1:property}': ${2:style}}"`                               |
| ngfor       | `*ngFor="let ${1:item} of ${2:list}"`                                     |
| ngif        | `*ngIf="${1:condition}"`                                                  |
| bscontainer | `<div class="container">$1</div>`                                         |
| bsrow       | `<div class="row">$1</div>`                                               |
| bsxs        | `<div class="col-xs-${1:6}">$2</div>`                                     |
| bssm        | `<div class="col-sm-${1:6}">$2</div>`                                     |
| bsmd        | `<div class="col-md-${1:6}">$2</div>`                                     |
| bslg        | `<div class="col-lg-${1:6}">$2</div>`                                     |
| bsbutton    | `<button type="button" class="btn ${1:btn-default}">${2:Button}</button>` |
| fa          | `<i class="fa fa-${1:home}"></i>`                                         |

## Typescript snippets
| Snippet     | Outcome                                                |
|-------------|--------------------------------------------------------|
| csl         | `console.log(${1:'here'});`                            |
| tsimport    | `import { ${1:Component} } from '${2:./}';`            |
| ngimport    | `import { ${1:Component} } from '@angular/${2:core}';` |
| nginput     | `@Input() ${1:variable} = ${2:value};`                 |
| ngoutput    | `@Output() ${1:variable} = new EventEmitter();`        |

**ngcomponent**

```
import { Component, OnInit } from '@angular/core';

@Component({
    selector: 'app-sample',
    templateUrl: './sample.component.html',
    styleUrls: ['./sample.component.less']
})
export class SampleComponent implements OnInit {
    constructor() {}

    ngOnInit() {}
}
```

**ngservice**

```
import { Injectable } from '@angular/core';

@Injectable()
export class MyService {

}
```

**ngmodule**

```
import { NgModule } from '@angular/core';
import { CommonModule } from '@angular/common';
import { FormsModule, ReactiveFormsModule } from '@angular/forms';

@NgModule({
    imports: [
        CommonModule,
        FormsModule,
        ReactiveFormsModule
    ],
    declarations: [],
    providers: []
})
export class AppModule { }
```

**ngroutes**

```
import { RouterModule } from '@angular/router';

const SampleRoutes = RouterModule.forChild([{
    path: '',
    component: SampleComponent,
    canActivate: [CanActivateRoute],
    data: {},
    children: [{
        path: '',
        redirectTo: 'overview',
        pathMatch: 'full'
    }, {
        path: 'overview',
        component: SampleOverviewComponent
    }, {
        path: 'details',
        component: SampleDetailsComponent
    }]
}];
```

## Javascript snippets

**describe**

```
describe('Description', () => {
    
});
```

**it**

```
it('Test', () => {
    
});
```

**expect-to-equal**

```
expect().to.equal();
```

## Javascript React snippets

**componenet**

```
import React from 'react'

class Component extends React.Component {
    render() {
        return <div />
    }
}

export default Component
```

## README.md snippet

**readme**

```markdown
# Project Title

One Paragraph of project description goes here

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

* [Docker](https://www.docker.com/) - Used to run the app

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

npm install

## Running the tests

Explain how to run the automated tests for this system

npm run test

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [NodeJS](https://nodejs.org/) - The web framework used
* [NPM](https://npmjs.com/) - Dependency Management

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Răzvan Muntian** - *Initial work* - [PurpleBooth](https://github.com/muntianrazvan)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
```

## MIT License snippet

**license-mit**

```
MIT License

Copyright (c) 2019 Razvan Muntian

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
