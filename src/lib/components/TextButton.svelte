<script lang="ts">
  export let content: string;
  export let disabled: boolean = false;
</script>

<button
  class="btn btn-primary"
  class:enabled={!disabled}
  class:disabled
  {disabled}
>
  <span role="img" aria-label="checkmark" class="px-2 py-1">{content}</span>
</button>
