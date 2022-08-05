<script>
  import { ExpansionPanels, MaterialApp } from 'svelte-materialify';
  import ShowCaseExpansionPanel from './components/ShowCaseExpansionPanel.svelte';
  import { experience } from './config';

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
    {#each experience as exp}
      <ShowCaseExpansionPanel item={exp} />
    {/each}
  </ExpansionPanels>
</MaterialApp>
