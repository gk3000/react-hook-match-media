# React hook to use Window.matchMedia() as media query in JavaScript 

With this hook you can determine the screen size and run any logic or apply styles based on that. Essentially it's a media queries inside JavaScript. 

## Installation

Run `npm i react-hook-match-media` or `yarn add react-hook-match-media` in the root of your React project


## Usage

In the component where you want to use this hook import it first 

```js
import {useMatchMedia} from 'react-hook-match-media';
```

then pass a condition for screen size which will evaluate to `true` or `false`: 

```js
const SomeComponent = (props)=>{
	const isSmallScreen = useMatchMedia('(max-width: 700px)');
}
```

Now the value if `isSmallScreen` would be a boolean, either `true` or `false` and you can use it for conditional rendering or in styles and it will respond to any changes of the screen size. For example in the snippet above it will be `true` for viewports smaller than 700px. 

---

Done at <a href='https://barcelonacodeschool.com'>Barcelona Code School</a>

