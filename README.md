# vue-slide

Vue carousel component for mobile

![1](https://user-images.githubusercontent.com/23690145/50532524-5c4a2700-0b55-11e9-9ea8-b8b4aa1911ae.gif)


### Install

```bash
yarn add @wyhaya/vue-slide
```

### Example

```vue
<template>
    <div>
        <slide :data="slide" />
    </div>
</template>

<script>
import slide from '@wyhaya/vue-slide'
export default {
    data() {
        return {
            slide: ['1.jpg', '2.jpg', '3.jpg']
        }
    },
    components: { slide }
}
</script>
```

### API

| Props        | Type                   | Default   | Explain                                      |
| -------------  | -------------   | -------------  | -------------                                |
| `:data`        | `string[] `     | `[]`           | Picture list                                 |
| `:time`        | `number`        | `3000ms`       | Timed scrolling time                         |
| `:spot`        | `boolean`       | `true`         | Whether to display the index                 |
| `:speed`       | `number`        | `300ms`        | Transition speed                             |
| `:type`        | `ease \| linear \| ease-in \| ...` | `ease` | Transition mode               |
| `:clockwise`   | `boolean`       | `true`         | Whether to scroll clockwise                  |
| `@click`       | `(index: number) => void` | `-`  | Callback function after clicking             |
| `@change`      | `(index: number) => void` | `-`  | Change the callback function after the index |
| `@prev`        | `(index: number) => void` | `-`  | Callback function after index forward        |
| `@next`        | `(index: number) => void` | `-`  | Callback function after index backwards      |

### More

* [React slide component](https://github.com/wyhaya/react-slide)
* [Slide without frame](https://github.com/wyhaya/slide)