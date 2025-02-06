<script lang="ts">
  import PageLayout from "$lib/layout/PageLayout.svelte";
  import Paragraph from "$lib/type/Paragraph.svelte";
  import Button from "$lib/buttons/Button.svelte";
  import Divider from "$lib/type/Divider.svelte";
  import AccentButton from "$lib/buttons/AccentButton.svelte";
  import Link from "$lib/type/Link.svelte";
</script>

<PageLayout>
  <h1 class="text-3xl text-type-emphasized mb-4 flex gap-3 text-center items-center justify-center font-semibold">[Lives]</h1>

  <Paragraph className="mt-3 mb-2">
    I sometimes livestream my practice sessions and shows along with other miscellaneous content using <Link href="https://obsproject.com/">OBS Studio</Link>.
  </Paragraph>

  <div class="flex flex-col gap-2">
    <div class="border border-mono-divider p-2 items-center flex flex-row justify-between">
      <div class="items-center flex flex-row gap-3">
        <img
          src="/yt-icon.png"
          loading="lazy"
          alt="YouTube Icon"
          class="h-10 w-auto" />
        YouTube
      </div>
      <AccentButton
        title="Go to YouTube"
        href="https://www.youtube.com/@manjar-o">
        View
      </AccentButton>
    </div>

    <div class="border border-mono-divider p-2 items-center flex flex-row justify-between">
      <div class="items-center flex flex-row gap-3">
        <img
          src="/ht-icon.png"
          loading="lazy"
          alt="HearThis Icon"
          class="h-10 w-auto" />
        HearThis
      </div>
      <AccentButton
        title="Go to HearThis"
        href="https://hearthis.at/manjar-o">
        View
      </AccentButton>
    </div>
  </div>

  <Divider />
  <div class="flex justify-between items-center">
    <Button
      title="Home"
      href="/">
      Home
    </Button>
    <Button
      title="Source code"
      href="https://github.com/itzcozi/manjar-o">
      Source code
    </Button>
  </div>
</PageLayout>
