# vscode-snippets
Snippets I use on a daily basis. These snippets can come handy if you use Bootstrap, Font Awesome, Angular or Typescript.

## HTML Snippets
| Snippet     | Outcome                                                                   |
|-------------|---------------------------------------------------------------------------|
| ngclass     | `[ngClass]="{'${1:class}': ${2:condition}}"`                              |
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
