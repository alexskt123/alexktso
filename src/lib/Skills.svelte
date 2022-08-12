<script>
  import { Row } from 'svelte-materialify';
  import SkillsChip from './components/SkillsChip.svelte';
  import { skills } from './config';
</script>

<Row class="mt-5 justify-center">
  {#each skills as skill}
    <SkillsChip name={skill} />
  {/each}
</Row>
