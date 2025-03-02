# Vue 3 Notes

## HTML

### Hello World
```vue
<template>
  <h1>Hello World</h1>
</template>
```

### Multiple roots
```vue
<template>
  <h1>Hello John</h1>
  <p>Lorem ipsum dolor...</p>
</template>
```

### Import
```vue
<script setup>
import HelloWorld from './components/HelloWorld';
</script>

<template>
  <HelloWorld />
</template>
```

### Slots

```vue
<template>
  <slot />
</template>
```
```vue
<template>
  <slot></slot>
</template>
```
```vue
<script setup>
import HelloWorld from './components/HelloWorld';
</script>

<template>
  <HelloWorld>This is some slot content!</HelloWorld>
</template>
```
---
```vue
<template>
  <slot>Fallback content</slot>
</template>
```

```vue
<script setup>
import HelloWorld from './components/HelloWorld';
</script>

<template>
  <HelloWorld></HelloWorld>
</template>
```

## CSS

### style attribute

```vue
<template>
  <h1 style="color: red;">Hello World</h1>
  <p>Lorem ipsum dolor...</p>
</template>
```

### style element

```vue
<template>
  <h1>Hello World</h1>
  <p>Lorem ipsum dolor...</p>
</template>

<style scoped>
h1 {
  color: red;
}
</style>
```

### class attribute

```vue
<template>
  <h1 class="heading">Hello World</h1>
</template>

<style scoped>
.heading {
  color: red;
}
</style>
```

## JS

### Variable
```vue
<script setup>
const count = 0;
</script>

<template>
  <button>Count: {{ count }}</button>
</template>
```

```vue
<script setup>
import { ref } from 'vue';
const count = ref(0);
</script>

<template>
  <button v-on:click="count++">Count: {{ count }}</button>
</template>
```

### Shorthand
```vue
<script setup>
import { ref } from 'vue';
const count = ref(0);
</script>

<template>
  <button @click="count++">Count: {{ count }}</button>
</template>
```

### Use function
```vue
<script setup>
import { ref } from 'vue';
const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <button @click="increment">Count: {{ count }}</button>
</template>
```

### Conditionals
```vue
<script setup>
import { ref } from 'vue';
const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <h1 v-if="show > 10">Good job!</h1>
  <h1 v-else-if="show > 5">Not bad</h1>
  <h1 v-else>Let's get started</h1>
  <button @click="increment">Count: {{ count }}</button>
</template>
```

### List
```vue
<script setup>
let id = 0;

const todos = [
  { id: id++, text: 'Learn HTML' },
  { id: id++, text: 'Learn JavaScript' },
  { id: id++, text: 'Learn Vue' }
]
</script>

<template>
<ul>
  <li v-for="todo in todos" :key="todo.id">
    {{ todo.text }}
  </li>
</ul>
</template>
```

### v-model
```vue
<script setup>
import { ref } from 'vue';
let id = 0;
const newTodo = ref('');

const todos = ref([
  { id: id++, text: 'Learn HTML' },
  { id: id++, text: 'Learn JavaScript' },
  { id: id++, text: 'Learn Vue' }
]);

function addTodo() {
  todos.value.push({ id: id++, text: newTodo.value });
  newTodo.value = '';
}
</script>

<template>
<ul>
  <li v-for="todo in todos" :key="todo.id">
    {{ todo.text }}
  </li>
</ul>
<input v-model="newTodo">
<button @click="addTodo">Add Todo</button>
</template>
```

### Props
```vue
<script setup>
const props = defineProps(['name'])
</script>

<template>
  <h1>Hello {{ name }}</h1>
</template>
```

```vue
<script setup>
const props = defineProps({
  name: String
})
</script>

<template>
  <h1>Hello {{ name }}</h1>
</template>
```

```vue
<script setup>
import HelloWorld from './components/HelloWorld';
</script>

<template>
  <HelloWorld name="John" />
</template>
```

### CSS + JS
```vue
<script setup>
import { ref } from 'vue';

const isActive = ref(true);
</script>

<template>
<h1 :class="{red: isActive}">Hello World</h1>
<button @click="isActive = !isActive">Toggle</button>
</template>

<style>
.red {
  color: red;
}
</style>
```

```vue
<script setup>
import { ref } from 'vue';

const isActive = ref(true);
const classObject = reactive({
  red: true
})
</script>

<template>
<h1 :class="classObject">Hello World</h1>
<button @click="isActive = !isActive">Toggle</button>
</template>

<style>
.red {
  color: red;
}
</style>
```

```vue
<script setup>
import { ref } from 'vue';

const isActive = ref(true);
const classObject = computed(() => ({
  red: isActive.value
}))
</script>

<template>
<h1 :class="classObject">Hello World</h1>
<button @click="isActive = !isActive">Toggle</button>
</template>

<style>
.red {
  color: red;
}
</style>
```
