<script lang="ts">
  import PageLayout from "$lib/layout/PageLayout.svelte";
  import Button from "$lib/buttons/Button.svelte";
</script>

<PageLayout>
  <h1 class="text-3xl text-type-emphasized mb-4 flex gap-3 text-center items-center justify-center font-semibold">
    <a
      href="/"
      title="Home"
      class="text-type-emphasized hover:text-type-emphasized hover:trasnparent hover:bg-transparent">
      [ManJar-O]
    </a>
  </h1>

  <div class="border border-mono-divider mb-4 p-2">

  </div>

  <div class="flex justify-between items-center">
    <Button
      title="About"
      href="/about">About</Button>
  </div>
</PageLayout>
