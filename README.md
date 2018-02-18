<p style="border-radius: 8px; background:#000" align="center"><img src="https://github.com/stagfoo/soshi/blob/master/build/soshi-bg.png?raw=true" width="150px" ></img></p>
<h1 align="center">Soshi</h1>
<p align="center">
  <a href="https://gitter.im/soshijs/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=body_badge">
  <img src="https://badges.gitter.im/soshijs/Lobby.svg" />
  </a>
  </p>
 <p align="center">
Experimental Component libray for any framework
</p>

# Includes
- 🕹️ Reusable component system
- 🍞 Simple interface
- 🐤 Teeny tiny
- ⚙️ Functional

## Run Example Usage
```
npm install
npm run start
```
## Built Components
these are built and in the showcase page

- Title
- Card
- Text List
- Button
- Image

## Usage
include soshi and choose a renderer, there are 3 included by default

```js
import Soshi from 'soshi'

const domComps = new Soshi({ dom: 'bel' }); //default renderer bel
domComps.r.title({text: 'Im a dom element'}); //HTMLElement

const vdomComps = new Soshi({ dom: 'vdom' }); //renderer virtual-dom
vdomComps.r.title({text: 'Im a vdom element'}); //virtual-dom object

const textComps = new Soshi({ dom: 'plaintext' }); //renderer plaintext
textComps.r.title({text: 'Im plaintext'}); //plaintext string
```

## Styling
These components will be styled by [fairybread](https://github.com/stagfoo/fairybread) in the Raeon Design Language (coming soon)

# Rendering System
Soshi works by using [hyperx](https://github.com/choojs/hyperx) and simple instancing to return your functional component

## Frameworks
### Tested
- **Bel** : Works fine
- **vdom**: Works fine
- **React** : Working using the createElement render function.
- **Vue**: Working with `plaintest` render, could be better
## Untested
- Angular: No tested
- Web Component
- [add your own framework!](https://github.com/stagfoo/soshi/issues/new)

# Idea behind 素子(soshi)
to create a simple extendable functional component system.
The end result should be a component that can be added to any framework.
