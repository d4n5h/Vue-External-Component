# Vue-External-Component
Utility library for importing external/remote Vue components. ([As seen here](https://markus.oberlehner.net/blog/distributed-vue-applications-loading-components-via-http/))

## Server setup:
https://github.com/d4n5h/Vue-Component-Repository

## Install:
```bash
$ npm install vue-external-component
```
## Example:
```vue
<template>
    <MyComponent/>
</template>

<script>
import externalComponent from 'vue-external-component';
const MyComponent = () => externalComponent(`http://localhost:8200/MyComponent/MyComponent.c9c0abb8e999d0e5654e.umd.min.js`);
export default {
  name: `App`,
  components: {
    MyComponent,
  },
};
</script>
```