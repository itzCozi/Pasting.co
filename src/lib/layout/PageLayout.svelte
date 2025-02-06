<script lang="ts">
  interface Props {
    children?: import("svelte").Snippet;
  }

  let { children }: Props = $props();
</script>

<div class="flex items-center justify-center p-4 min-h-screen">
  <div class="mx-auto md:w-[32rem] w-[25rem] h-full border border-mono-divider p-4">
    {@render children?.()}
  </div>
</div>
