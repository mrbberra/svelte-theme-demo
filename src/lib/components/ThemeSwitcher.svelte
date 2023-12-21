<script lang="ts">
  import { themeStore } from "../stores/ThemeStore";

  const updateTheme = (theme: string) => {
    $themeStore = theme;
  };
</script>

<div class="dropdown mb-5">
  <button
    class="btn btn-secondary dropdown-toggle"
    type="button"
    data-bs-toggle="dropdown"
    aria-expanded="false"
  >
    Theme: {$themeStore}
  </button>
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#" on:click={() => updateTheme("duplo")}>Duplo</a></li>
    <li><a class="dropdown-item" href="#" on:click={() => updateTheme("lego")}>Lego</a></li>
    <li><a class="dropdown-item" href="#" on:click={() => updateTheme("adult")}>Adult</a></li>
  </ul>
</div>
