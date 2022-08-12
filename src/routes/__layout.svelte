<script>
  import Drawer from '$lib/Drawer.svelte';
  import { isMobile } from 'is-mobile';
  import { Jumper } from 'svelte-loading-spinners';
  import { onMount } from 'svelte';
  import { Row } from 'svelte-materialify';
  import '../app.css';

  let ready = false;

  onMount(() => (ready = true));
</script>

{#if ready}
  {#if !isMobile()}
    <Drawer />
  {/if}
  <div style="background-color:snow;min-height:100vh">
    <slot />
  </div>
{:else}
  <Row class="d-flex justify-center">
    <Jumper size="60" color="#FF3E00" unit="px" duration="1s" />
  </Row>
{/if}
