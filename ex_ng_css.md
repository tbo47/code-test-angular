Coding exercise.

## install

Install nodejs 20 via [nvm](https://github.com/nvm-sh/nvm), vscode, git.

Install angular cli:
`npm install -g @angular/cli`

## code generation

Create an Angular project:
`ng new code-test-angular --style sass --ssr false`

Open the project with vscode.

Generate components
```
ng generate component header
ng generate component content
ng generate component menu
ng generate service my-service
```



## task #1

```
                                                                
 ┌─┬───────────────────────────────────────────────────────┬─┐  
 │ ├───────────────────────────────────────────────────────┤ │  
 │ │                                                       │ │  
 │ │                header                                 │ │  
 │ │                                                       │ │  
 │ │                                                       │ │  
 │ │                                                       │ │  
 │ └───────────────────────────────────────────────────────┘ │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                   ┌──────────────────────┐                │  
 │                   │                      │                │  
 │                   │                      │                │  
 │                   │                      │                │  
 │                   │      content         │                │  
 │                   │                      │                │  
 │                   │                      │                │  
 │                   │                      │                │  
 │                   │                      │                │  
 │                   └──────────────────────┘                │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │                                                           │  
 │ ┌──────────────────────────────────────────────────────┐  │  
 │ │┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼  menu ┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼┼│  │  
 └─┴──────────────────────────────────────────────────────┴──┘  
                                                                
```


The header must be visible when we scroll down the page. It must have a logo on the left and a logo on the right. (using css flex)

The content is centered in the middle of the page. (using css flex)

The menu must have round corners and is fixed in the bottom of the page.



## task #2

TODO inter component and service communication