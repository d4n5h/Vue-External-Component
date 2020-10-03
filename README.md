# Vue-External-Component
Utility library for importing external/remote Vue components. ([As seen here](https://markus.oberlehner.net/blog/distributed-vue-applications-loading-components-via-http/))

## Install:
```bash
$ npm install vue-external-component
```
## Example:
```javascript
import externalComponent from 'vue-external-component';

const MyComponent = () => externalComponent('http://localhost:8200/MyComponent/MyComponent.c9c0abb8e999d0e5654e.umd.min.js');

export default {
  name: 'MyOtherComponent',
  components: {
    MyComponent,
  }
}
```