<script lang="ts">
  export interface Props {
    className?: string;
    onInput?: (event: Event) => void;
    placeholder?: string;
    value?: string;
    title?: string;
  }

  let { className = "", onInput = () => {}, placeholder = "", value = "", title }: Props = $props();
</script>

<input
  class={`text-type-dimmed bg-transparent border border-mono-divider py-1 px-2 focus:border-type-footer focus:outline-none transition duration-200 ease-in-out ${className}`}
  oninput={onInput}
  title={title}
  placeholder={placeholder}
  bind:value={value} />
