<script lang="ts">
  export let variant: string | "texticon" | "icon" | "text" = "text";
  export let disabled: boolean | true | false = false;
</script>

{#if variant === "texticon"}
  <button
    disabled={disabled}
    class="flex items-center gap-3 bg-neutral-900 h-[36px] pl-2 pr-4 py-auto rounded-md text-[14px] font-sans font-semibold bg-opacity-75 hover:bg-neutral-800 border border-white border-opacity-5 transition-all duration-300 ease-in-out"
  >
    <slot />
  </button>
{:else if variant === "icon"}
  <button
  disabled={disabled}
    class="bg-neutral-900 h-[36px] w-[36px] rounded-md text-[14px] font-sans font-semibold flex items-center justify-center bg-opacity-75 hover:bg-neutral-800 border border-white border-opacity-5 transition-all duration-300 ease-in-out"
  >
    <slot />
  </button>
{:else if variant === "text"}
  <button
  disabled={disabled}
    class="bg-neutral-900 h-[36px] px-4 py-auto rounded-md text-[14px] font-sans font-semibold bg-opacity-75 hover:bg-neutral-800 border border-white border-opacity-5 transition-all duration-300 ease-in-out"
  >
    <slot />
  </button>
{/if}
