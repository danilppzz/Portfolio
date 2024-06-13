<!-- TuComponente.svelte -->
<script>
  import IconArchive from "../components/icons/IconArchive.svelte";
  import IconCase from "../components/icons/IconCase.svelte";
  import IconCross from "../components/icons/IconCross.svelte";
  import IconMail from "../components/icons/IconMail.svelte";
  import IconPin from "../components/icons/IconPin.svelte";
  import IconPower from "../components/icons/IconPower.svelte";
  import IconShare from "../components/icons/IconShare.svelte";
  import IconStar from "../components/icons/IconStar.svelte";
  import IconTick from "../components/icons/IconTick.svelte";
  // Exporta los props "title" e "icon"
  export let title = "";
  export let icon = 0;

  // Define un array de componentes para utilizarlos como íconos
  const icons = ["", IconArchive, IconCase, IconCross, IconMail, IconPin, IconPower, IconShare, IconStar, IconTick];
</script>

<section class="max-w-3xl mx-auto mt-14">
  <div class="flex items-center mb-4">
    {#if icon >= 0 && icon < icons.length}
      <svelte:component this={icons[icon]} class="mr-2 w-6 h-6" />
    {/if}
    {#if title}
      <h2 class="font-bold font-mono text-lg">{title}</h2>
    {/if}
  </div>
  <slot />
</section>
