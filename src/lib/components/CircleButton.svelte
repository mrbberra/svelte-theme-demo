<script lang="ts">
  export let disabled: boolean = false;
  export let color: string = "primary";
  export let icon: "check" | "volume-up-fill" | "stop-fill";
</script>

<button class="btn rounded-circle p-1 bg-es-{color}" class:disabled {disabled}>
  <i class="bi-{icon} text-white d-flex fs-1"></i>
</button>
