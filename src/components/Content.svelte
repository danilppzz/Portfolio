<script>
  import IconStar from "./icons/IconStar.svelte";
</script>

<div class="w-full flex flex-col whitespace-nowrap rounded-lg text-sm font-medium font-mono focus-visible:outline-none focus-visible:ring-1 disabled:pointer-events-none disabled:opacity-50 dark:focus-visible:ring-neutral-700 focus-visible:ring-neutral-500 border border-neutral-200 bg-white shadow-sm dark:border-neutral-800 dark:bg-neutral-900 group hover:border-white hover:border-opacity-20 transition-colors">
  <slot />
</div>
