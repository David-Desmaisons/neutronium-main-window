# Neutronium_main_window


[![Npm download](https://img.shields.io/npm/dt/neutronium_main_window.svg?maxAge=2592000)](https://www.npmjs.com/package/neutronium_main_window)
[![Npm version](https://img.shields.io/npm/v/neutronium_main_window.svg?maxAge=2592000)](https://www.npmjs.com/package/neutronium_main_window)
[![MIT License](https://img.shields.io/github/license/David-Desmaisons/neutronium_main_window.svg)](https://github.com/David-Desmaisons/neutronium_main_window/blob/master/LICENSE)


Vue component (Vue.js 2.0) to manage [Neutronium](https://github.com/David-Desmaisons/Neutronium) main view


Tipical use:
HTML:
```html
  <neutronium-main-view name="fade" :window="viewModel.__window__">
      <img src="./assets/logo.png">
      ...
  </neutronium-main-view>
```

javascript:

```javascript
import NeutroniumMainWindow from 'NeutroniumMainWindow.vue'

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
