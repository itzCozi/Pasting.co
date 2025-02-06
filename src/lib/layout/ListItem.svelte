<script lang="ts">
  interface Props {
    className?: string | undefined;
    href: string;
    text: string;
  }

  let { className = "", href, text }: Props = $props();
</script>

<li class={`flex flex-row gap-2 ${className}`}>
  <a
    {href}
    class="w-full text-sm duration-200 ease-in-out"
    target="_blank">{text}</a>
</li>
