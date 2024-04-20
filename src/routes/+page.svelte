<script lang="ts">
  let counter = 0;

  const increment = (val: number = 0) => {
    if (val > 0) {
      counter += val;
    } else {
      counter++;
    }
  };
  const decrement = () => {
    counter++;
  };
</script>

<h1>Welcome to SvelteKit</h1>
<button on:click={() => increment()}>Count : {counter}</button>
<button on:click={() => increment(10)}>Add 10</button>
