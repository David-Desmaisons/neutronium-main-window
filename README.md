# Neutronium_main_window


[![Npm download](https://img.shields.io/npm/dt/neutronium-main-window.svg?maxAge=2592000)](https://www.npmjs.com/package/neutronium-main-window)
[![Npm version](https://img.shields.io/npm/v/neutronium-main-window.svg?maxAge=2592000)](https://www.npmjs.com/package/neutronium-main-window)
[![MIT License](https://img.shields.io/github/license/David-Desmaisons/neutronium-main-window.svg)](https://github.com/David-Desmaisons/neutronium-main-window/blob/master/LICENSE)


Vue component (Vue.js 2.0) to manage [Neutronium](https://github.com/David-Desmaisons/Neutronium) main view


##Tipical use:
HTML:
```html
  <neutronium-main-view name="fade" :main-view-model="viewModel">
      <img src="./assets/logo.png">
      ...
  </neutronium-main-view>
```

javascript:

```javascript
import NeutroniumMainWindow from 'neutronium-main-window.vue'

export default {
  components:{
    NeutroniumMainWindow
  },
  //....
```

CSS:
```css
.fade-enter-active, .fade-leave-active {
  transition: opacity .2s
}
.fade-enter, .fade-leave-active {
  opacity: 0
}
```

This component will allow transition when displaying a given view model.
See [Neutronium documentation](https://github.com/David-Desmaisons/Neutronium/wiki) and [NeutroniumDemo](https://github.com/David-Desmaisons/NeutroniumDemo) for more details.


##Instalation

```
npm install --save neutronium-main-window
```