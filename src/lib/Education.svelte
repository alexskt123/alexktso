<script>
  import { ExpansionPanels, MaterialApp } from 'svelte-materialify';
  import ShowCaseExpansionPanel from './components/ShowCaseExpansionPanel.svelte';
  import { education } from './config';

  //   let value = [0];
  let about = { index: '', active: '' };
  /**
   * @param {{ detail: { index: string; active: string; }; }} e
   */
  function onChange(e) {
    about = e.detail;
  }
</script>

<MaterialApp>
  <ExpansionPanels on:change={onChange} style={'width:100%'} class="mt-5">
    {#each education as edu}
      <ShowCaseExpansionPanel item={edu} />
    {/each}
  </ExpansionPanels>
</MaterialApp>
