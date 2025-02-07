<script lang="ts">
  import PageLayout from "$lib/layout/PageLayout.svelte";
  import Paragraph from "$lib/type/Paragraph.svelte";
  import BigButton from "$lib/buttons/Button.svelte";
  import Button from "$lib/buttons/Button.svelte";
  import Divider from "$lib/type/Divider.svelte";
  import ListItem from "$lib/layout/ListItem.svelte";
  import Input from "$lib/type/Input.svelte";
  import TextArea from "$lib/type/TextArea.svelte";
  import Checkbox from "$lib/buttons/Checkbox.svelte";
  import AccentButton from "$lib/buttons/AccentButton.svelte";
</script>

<PageLayout>
  <h1 class="text-3xl text-type-emphasized mb-4 flex gap-3 text-center items-center justify-center font-semibold">Pasting.co</h1>

  <TextArea className="w-full h-32" placeholder="Type something here..." />

  <div class="flex flex-row gap-2">
    <Input
      title="Paste URL"
      placeholder="Custom URL"
      className="w-full py-2" />
    <Input
      title="Edit Password"
      placeholder="Edit Password"
      className="w-full py-2" />

    <!--
      <div>
        Here we add hella icons to add onClick events to so like burn after read, password protected
      </div>
    -->
  </div>

  <Divider />
  <div class="flex justify-between items-center">
    <AccentButton
      className="hover:bg-[#f44646] hover:text-white"
      title="Livestreams"
      href="/live">
      Delete
    </AccentButton>
    <AccentButton
      title="Source code"
      href="https://github.com/itzcozi/manjar-o">
      Publish
    </AccentButton>
  </div>
</PageLayout>
