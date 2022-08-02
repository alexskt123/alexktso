<script>
  import { Chip, ExpansionPanel, ExpansionPanels, MaterialApp } from 'svelte-materialify';

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
    <ExpansionPanel>
      <span slot="header">
        <strong>The Hong Kong University of Science & Technology</strong>
      </span>
      <ul class="mt-5">
        <li>Bachelor of Engineering in Computer Science</li>
      </ul>
    </ExpansionPanel>
    <ExpansionPanel>
      <span slot="header">
        <strong>The University of London</strong>
      </span>
      <ul class="mt-5">
        <li>Bachelor of Laws</li>
      </ul>
    </ExpansionPanel>
    <ExpansionPanel>
      <span slot="header">
        <strong>The University of Hong Kong</strong>
      </span>
      <ul class="mt-5">
        <li>Postgraduate Certificate in Laws</li>
      </ul>
    </ExpansionPanel>
  </ExpansionPanels>
</MaterialApp>
