<script lang="ts">
  import { onMount } from "svelte";
  import { themeStore } from "../lib/stores/ThemeStore";
  import "../app.scss";

  let root: HTMLElement;

  onMount(() => {
    root = document.documentElement;
  });

  const themes = ["duplo", "lego", "adult"];

  const setTheme: any = (currentTheme: string) => {
    for (const theme of themes) {
      if (currentTheme === theme) {
        root.classList.add(theme);
      } else {
        root.classList.remove(theme);
      }
    }
  };

  $: root && setTheme($themeStore);
</script>

<slot />
