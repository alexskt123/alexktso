<script>
  import { ExpansionPanel, ExpansionPanels, MaterialApp } from 'svelte-materialify';

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
  <ExpansionPanels on:change={onChange} style={'width:100%'} class="mt-10">
    <ExpansionPanel>
      <span slot="header">
        <strong>HKT Limited - Senior System Analyst</strong>
      </span>
      <ul class="mt-5">
        <li>Involved in one of the largest emerging technology projects in Hong Kong</li>
        <li>Conducted system design of various modules in the core application system</li>
        <li>Led developers from Offshore Development Centers</li>
        <li>Co-operated with vendors for the system development and architecture design</li>
      </ul>
    </ExpansionPanel>
    <ExpansionPanel>
      <span slot="header">
        <strong>Bank Consortium Trust Company Limited - Senior Analyst Programmer</strong>
      </span>
      <ul class="mt-5">
        <li>
          Implemented various system enhancements and performed ad hoc system maintenance tasks
        </li>
        <li>
          Collected user requirements with Systems Analysts and provided functional specifications
        </li>
        <li>Assisted, coached and gave technical advice to programmers</li>
        <li>Developed and maintained RESTful APIs</li>
      </ul>
    </ExpansionPanel>
    <ExpansionPanel>
      <span slot="header">
        <strong>Ricoh Hong Kong Limited - Analyst Programmer</strong>
      </span>
      <ul class="mt-5">
        <li>Assisted in the Enterprise Resource Planning (ERP) Modernization project</li>
        <li>
          Maintained the core system by performing bug fixing, data patching, housekeeping and
          system enhancements
        </li>
      </ul>
    </ExpansionPanel>
    <ExpansionPanel>
      <span slot="header">
        <strong>Aedify Technology Limited - Web Programmer</strong>
      </span>
      <ul class="mt-5">
        <li>Implemented the registration system of the website with Facebook API</li>
        <li>Built the interface and the functionality of the website using MVC infrastructure</li>
      </ul>
    </ExpansionPanel>
  </ExpansionPanels>
</MaterialApp>
