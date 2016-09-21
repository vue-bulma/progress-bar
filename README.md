# ProgressBar

ProgressBar component for Vue Bulma.


## Installation

```
$ npm install vue-bulma-progress-bar --save
```


## Examples

```vue
<template>
  <progress-bar :type="'success'" :size="'large'" :value="dynamicValue" :max="100" :show-label="true"></progress-bar>
</template>

<script>
import ProgressBar from 'vue-bulma-progress-bar'

export default {
  components: {
    ProgressBar
  },

  data () {
    return {
      dynamicValue: 60
    }
  },

  methods: {
    plus () {
      if (this.dynamicValue === 100) return
      this.dynamicValue += 10
    },

    minus () {
      if (this.dynamicValue === 0) return
      this.dynamicValue -= 10
    }
  }

}
</script>
```



## Badges

![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

---

> [fundon.me](https://fundon.me) &nbsp;&middot;&nbsp;
> GitHub [@fundon](https://github.com/fundon) &nbsp;&middot;&nbsp;
> Twitter [@_fundon](https://twitter.com/_fundon)
