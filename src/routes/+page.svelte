<script lang="ts">
  import CloseButton from "../lib/components/CloseButton.svelte";
  import CircleButton from "../lib/components/CircleButton.svelte";
  import TextButton from "../lib/components/TextButton.svelte";
  import ThemeSwitcher from "$lib/components/ThemeSwitcher.svelte";
</script>

<div class="container p-5">
  <ThemeSwitcher />
  <div class="row border border-dark rounded-2">
    <div class="col justify-content-center">
      <div class="my-3">
        <TextButton content="Hello" />
      </div>
      <div class="my-3">
        <CloseButton />
      </div>
      <div class="my-3">
        <CircleButton icon="stop-fill" color="yellow" />
      </div>
    </div>
  </div>
</div>
