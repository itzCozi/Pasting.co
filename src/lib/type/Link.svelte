<script lang="ts">
  export interface Props {
    className?: string;
    href?: string;
    title?: string;
    children?: import("svelte").Snippet;
  }

  let { className = "", href = "", title = "", children }: Props = $props();
</script>

<a
  class={`duration-200 ease-in-out ${className}`}
  {href}
  {title}>
  {@render children?.()}
</a>
