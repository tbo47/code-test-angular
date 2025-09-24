Coding exercise. The result should be a github project.

## install

Install nodejs via [nvm](https://github.com/nvm-sh/nvm), vscode/cursor, git.

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

Note: To be able to use `<app-header></app-header>` in `app.component.html` you have to add `HeaderComponent` to the `imports` array in `app.component.ts`

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

The header must be visible when we scroll down the page.

## task #2

Let's create a array of football players.

```javascript
footballers = signal([
  { name: "Messi", club: "Barcelona", continent: "South America" },
  { name: "Ronaldo", club: "Juventus", continent: "Europe" },
  { name: "Neymar", club: "PSG", continent: "South America" },
  { name: "Kylian Mbappé", club: "Real Madrid", continent: "Europe" },
  { name: "Erling Haaland", club: "Manchester City", continent: "Europe" },
  { name: "Kevin De Bruyne", club: "Manchester City", continent: "Europe" },
  { name: "Robert Lewandowski", club: "Barcelona", continent: "Europe" },
  { name: "Mohamed Salah", club: "Liverpool", continent: "Africa" },
  { name: "Luka Modrić", club: "Real Madrid", continent: "Europe" },
  { name: "Harry Kane", club: "Bayern Munich", continent: "Europe" },
  { name: "Antoine Griezmann", club: "Atlético Madrid", continent: "Europe" },
  { name: "Vinícius Júnior", club: "Real Madrid", continent: "South America" },
  { name: "Jude Bellingham", club: "Real Madrid", continent: "Europe" },
  { name: "Bernardo Silva", club: "Manchester City", continent: "Europe" },
  { name: "Son Heung-min", club: "Tottenham Hotspur", continent: "Asia" },
  { name: "Bukayo Saka", club: "Arsenal", continent: "Europe" },
  { name: "Martin Ødegaard", club: "Arsenal", continent: "Europe" },
  { name: "Pedri", club: "Barcelona", continent: "Europe" },
  { name: "Gavi", club: "Barcelona", continent: "Europe" },
]);
selectedFootballer = signal<{ name: string, club: string, continent: string } | null>(null)
```

Display the list of the footballers in the `header` component using the new `@for` syntax.

When we click on the name of a  player in the `header`, we want the `selectedFootballer` to be updated and be displayed in the `<app-content>` component.

## bonus task

Create a `computed` which will "react" to the `footballers` signal. It displays the footballers grouped by continent.