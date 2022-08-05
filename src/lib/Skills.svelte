<script>
  import { Row, MaterialApp } from 'svelte-materialify';
  import SkillsChip from './components/SkillsChip.svelte';
  import { skills } from './config';
</script>

<MaterialApp>
  <Row class="mt-5">
    {#each skills as skill}
      <SkillsChip name={skill} />
    {/each}
  </Row>
</MaterialApp>
