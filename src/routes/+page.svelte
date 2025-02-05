<script lang="ts">
  import PageLayout from "$lib/layout/PageLayout.svelte";
  import Paragraph from "$lib/type/Paragraph.svelte";
  import BigButton from "$lib/buttons/Button.svelte";
  import Button from "$lib/buttons/Button.svelte";
  import Divider from "$lib/type/Divider.svelte";
  import ListItem from "$lib/layout/ListItem.svelte";
</script>

<PageLayout>
  <h1 class="text-3xl text-type-emphasized mb-4 flex gap-3 text-center items-center justify-center font-semibold">[ManJar-O]</h1>

  <Paragraph className="mt-3 mb-2">
    ManJar-O (Cooper Ransom) is a passionate 16-year-old software developer and bedroom DJ hailing from Charlotte, North Carolina. With a strong foundation in web development, Cooper is now expanding
    his creative mediums by joining the world of music production and mixing. His journey is fueled by a relentless drive to blend technology with a new minimal artistic expression.
  </Paragraph>

  <div class="border border-mono-divider mb-4 p-1">
    <ListItem
      href="https://soundcloud.com/manjar-o"
      text="SoundCloud" />
    <ListItem
      href="https://hearthis.at/manjar-o"
      text="HearThis.at" />
    <ListItem
      href="https://www.youtube.com/@manjar-o"
      text="YouTube" />
  </div>

  <div class="flex flex-row gap-2">
    <BigButton
      title="Email"
      onClick={() => window.open("mailto:dev@wyzie.ru")}
      className="w-full py-2">
      dev@wyzie.ru
    </BigButton>

    <BigButton
      title="Phone number"
      onClick={() => window.open("tel:9802979605")}
      className="w-full py-2">
      (980)-297-9605
    </BigButton>
  </div>

  <Divider />

  <div class="flex justify-end items-center">
    <Button
      title="Source code"
      href="https://github.com/itzcozi/manjar-o">
      Source code
    </Button>
  </div>
</PageLayout>
