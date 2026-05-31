<script lang="ts">
  let count = $state(0);
</script>

<div class="counter">
  <h1>Counter</h1>
  <p class="display">{count}</p>
  <div class="buttons">
    <button onclick={() => count++}>+</button>
    <button onclick={() => count--}>-</button>
    <button onclick={() => count = 0}>Reset</button>
  </div>
</div>

<style>
  .counter {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 80vh;
    font-family: system-ui, sans-serif;
  }
  .display {
    font-size: 4rem;
    font-weight: bold;
    margin: 1rem 0;
    color: #333;
  }
  .buttons {
    display: flex;
    gap: 0.75rem;
  }
  button {
    font-size: 1.5rem;
    padding: 0.5rem 1.25rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    background: #f5f5f5;
    cursor: pointer;
    transition: background 0.15s;
  }
  button:hover {
    background: #e0e0e0;
  }
  button:active {
    background: #ccc;
  }
</style>
