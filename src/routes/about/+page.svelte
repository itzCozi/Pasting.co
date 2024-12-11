<script lang="ts">
  import PageLayout from "$lib/layout/PageLayout.svelte";
  import Paragraph from "$lib/type/Paragraph.svelte";
  import BigButton from "$lib/buttons/Button.svelte";
  import Button from "$lib/buttons/Button.svelte";
  import Divider from "$lib/type/Divider.svelte";
  import { goto } from "$app/navigation";
</script>

<PageLayout>
  <h1 class="text-3xl text-type-emphasized mb-4 flex gap-3 text-center items-center justify-center font-semibold">
    <a
      href="/"
      title="Home"
      class="text-type-emphasized hover:text-type-emphasized hover:trasnparent hover:bg-transparent">
      About [ManJar-O]
    </a>
  </h1>
  <Paragraph className="mt-3 mb-2">
    ManJar-O is a passionate 16-year-old software developer and bedroom DJ hailing from Charlotte, North Carolina. With a strong foundation in web development, ManJar-O is now expanding his creative mediums by joining the world of music production and mixing. His journey is fueled by a relentless drive to blend technology with a new artistic expression.
  </Paragraph>
  <BigButton
    title="Email"
    onClick={() => window.open("mailto:dev@wyzie.ru")}
    className="w-full py-2">
    Email Me
  </BigButton>
  <Divider />
  <div class="flex justify-between items-center">
    <Button
      title="Home"
      href="/">
      Home
    </Button>
    <Button
      title="Source code"
      href="https://github.com/itzcozi/365">
      Source code
    </Button>
  </div>
</PageLayout>
