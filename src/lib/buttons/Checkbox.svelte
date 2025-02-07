<script lang="ts">
  export let title: string;
  export let checked: boolean = false;

  function toggle() {
    checked = !checked;
  }
</script>

<label class="flex items-center cursor-pointer">
  <input type="checkbox" bind:checked on:change={toggle} class="hidden" />
  <span class="w-4 h-4 border-2 border-accent rounded-sm flex items-center justify-center mr-2">
    {#if checked}
      <svg class="w-3 h-3 text-accent" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414 0L9 11.586 6.707 9.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7a1 1 0 000-1.414z" clip-rule="evenodd" />
      </svg>
    {/if}
  </span>
  {title}
</label>

<style>
  .border-accent {
    border-color: var(--color-mono-accent);
  }
  .text-accent {
    color: var(--color-mono-accent);
  }
</style>
