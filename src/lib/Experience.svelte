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
  <ExpansionPanels on:change={onChange} style={"width:100%"} class="mt-10">
    <ExpansionPanel>
      <span slot="header">
        <strong>HKT Limited - Senior System Analyst</strong>
      </span>
      <ul class="mt-5">
        <li>
            Conducted system design of various modules (i.e. Payment, Dual Input and Withdrawal) in the core application system (CAS) and developed corresponding Front End Web Application and Back End APIs
        </li>
        <li>
            Submitted system design documents to the Mandatory Provident Fund Schemes Authority (MPFA) and liaised with MPFA for the agreement of the system design
        </li>
        <li>
            Managed and coordinated with vendor to develop Payment Instruction Gateway (PIG) for CAS
        </li>
        <li>
            Studied the system feasibility using Maven, Java, Spring Boot, Message Queue, React Js and Oracle
        </li>
        <li>
            Led developers from Offshore Development Centers based in Malaysia and Philippines
        </li>
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
        <li>
            Assisted, coached and gave technical advice to programmers
        </li>
        <li>
            Developed and maintained RESTful APIs
        </li>
      </ul>
    </ExpansionPanel>
  </ExpansionPanels>
</MaterialApp>
