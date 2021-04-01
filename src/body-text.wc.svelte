<svelte:options tag="pg-body-text" />

<p class="body-text">
  <slot />
</p>

<style>
  .body-text {
    color: var(--secondary-color);
    font-size: 18px;
  }
</style>
