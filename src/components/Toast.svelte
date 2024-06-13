<script>
  import IconCross from "./icons/IconCross.svelte";
  export let title = "Cookies";
</script>

<div
  class="items-center space-x-3 whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-1 disabled:pointer-events-none disabled:opacity-50 dark:focus-visible:ring-neutral-700 focus-visible:ring-neutral-500 border border-neutral-200 bg-white shadow-sm dark:border-neutral-800 dark:bg-neutral-900 h-auto w-auto px-2 py-2 group"
>
  <div class="flex items-center justify-between w-full">
    <p class="ml-2">{title}</p>
    <span
      class="flex items-center w-6 h-6 justify-center rounded-full transition-colors cursor-pointer dark:bg-neutral-900 dark:hover:bg-neutral-800 dark:hover:text-neutral-50 dark:hover:border-neutral-700/50"
    >
      <svelte:component this={IconCross} class="w-4 h-4" />
    </span>
  </div>
  <p class="ml-2">You must accept the cookies for use some extra features of the web.</p>
</div>
