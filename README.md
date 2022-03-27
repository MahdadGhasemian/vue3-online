# vue3-online

A Component for show internet connection

![Screenshot](https://github.com/MahdadGhasemian/vue3-online/blob/main/vue-detect-internet-connection.gif)

## Installation

### npm

```bash
npm i vue3-online --save
```

### Usage

main.js

```javascript
import { createApp } from "vue";
import App from "./App.vue";
import Vue3Online from "vue3-online";

createApp(App).component("online-offline", Vue3Online).mount("#app");
```

Or in component

```html
<template>
  <div>
    <online-offline> Is Online </online-offline>
  </div>
</template>

<script>
  import Vue3Online from "vue3-online";
  export default {
    components: {
      OnlineOffline: Vue3Online,
    },
  };
</script>
```

## Examples

### Example1

```vue
<template>
  <div>
    <online-offline>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-full w-5"
        viewBox="0 0 20 20"
        fill="currentColor"
      >
        <path
          fill-rule="evenodd"
          d="M17.778 8.222c-4.296-4.296-11.26-4.296-15.556 0A1 1 0 01.808 6.808c5.076-5.077 13.308-5.077 18.384 0a1 1 0 01-1.414 1.414zM14.95 11.05a7 7 0 00-9.9 0 1 1 0 01-1.414-1.414 9 9 0 0112.728 0 1 1 0 01-1.414 1.414zM12.12 13.88a3 3 0 00-4.242 0 1 1 0 01-1.415-1.415 5 5 0 017.072 0 1 1 0 01-1.415 1.415zM9 16a1 1 0 011-1h.01a1 1 0 110 2H10a1 1 0 01-1-1z"
          clip-rule="evenodd"
        />
      </svg>
    </online-offline>
  </div>
</template>
```

### Example2

```vue
<template>
  <div>
    <online-offline> Is Online </online-offline>
  </div>
</template>
```

## Change log

### 0.0.3 (2022-03-27)

- update readme file

### 0.0.2 (2022-03-27)

- add readme file

### 0.0.1 (2022-03-27)

- first release

<br />
<br />
<br />
<hr />
