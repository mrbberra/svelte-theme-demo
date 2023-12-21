<script lang="ts">
  export let disabled: boolean = false;
</script>

<button
  class="btn btn-close"
  class:enabled={!disabled}
  class:disabled
  {disabled}
>
</button>
