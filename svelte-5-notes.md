# Svelte 5 Notes

## HTML

### Hello World
```svelte
<h1>Hello World</h1>
```

### Multiple roots
```svelte
<h1>Hello John</h1>
<p>Lorem ipsum dolor...</p>
```

### Import
```svelte
<script>
import HelloWorld from './HelloWorld.svelte';
</script>

<HelloWorld />
```

## CSS

### style attribute

```svelte
<h1 style="color: red;">Hello World</h1>
<p>Lorem ipsum dolor...</p>
```

### style element

```svelte
<h1>Hello World</h1>
<p>Lorem ipsum dolor...</p>

<style>
h1 {
  color: red;
}
</style>
```

### class attribute

```svelte
<h1 class="heading">Hello World</h1>

<style>
.heading {
  color: red;
}
</style>
```

## JS

### Variable
```svelte
<script>
let count = 0;
</script>

<button>Count: { count }</button>
```

### Reactive
```svelte
<script>
let count = $state(0);
</script>

<button onclick="count++">Count: { count }</button>
```

### Use function
```svelte
<script>
let count = $state(0);

function increment() {
  count++;
}
</script>

<button onclick={increment}>Count: { count }</button>
```

### Conditionals
```svelte
<script>
let count = $state(0);

function increment() {
  count++;
}
</script>

{#if count > 10}
<h1>Good job!</h1>
{:else if count > 5}
<h1>Not bad</h1>
{:else}
<h1>Let's get started</h1>
{/if}
<button onclick={increment}>Count: { count }</button>
```

### List
```svelte
<script>
let id = 0;

const todos = [
  { id: id++, text: 'Learn HTML' },
  { id: id++, text: 'Learn JavaScript' },
  { id: id++, text: 'Learn Svelte' }
]
</script>


<ul>
  {#each todos as todo}
    <li>{ todo.text }</li>
  {/each}
</ul>
```

### bind:value
```svelte
<script>
let id = 0;
let newTodo = $state('');

const todos = $state([
  { id: id++, text: 'Learn HTML' },
  { id: id++, text: 'Learn JavaScript' },
  { id: id++, text: 'Learn Svelte' }
]);

function addTodo() {
  todos.push({ id: id++, text: newTodo });
  newTodo = '';
}
</script>


<ul>
  {#each todos as todo}
    <li>{ todo.text }</li>
  {/each}
</ul>
<input bind:value={newTodo}>
<button onclick={addTodo}>Add Todo</button>
```

### Props
```svelte
<script>
let { name } = $props();
</script>

<h1>Hello { name }</h1>
```

```svelte
<script>
let props = $props();
</script>

<h1>Hello { props.name }</h1>
```

```svelte
<script>
import HelloWorld from './HelloWorld.svelte';
</script>

<HelloWorld name="John" />
```
