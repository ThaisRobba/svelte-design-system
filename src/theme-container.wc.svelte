<svelte:options tag="pg-theme-container" />

<script>
  export let primary = "green";
  export let secondary = "red";
</script>

<div style="--primary-color: {primary};--secondary-color: {secondary}">
  <slot />
</div>
