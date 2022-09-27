<script>
  import { Tabs, Tab, TabContent, Row } from 'svelte-materialify';
  import SkillsChip from './components/SkillsChip.svelte';
  import { skills } from './config';

  const tabs = ['Front-end', 'Back-end', 'Database', 'Cloud', 'CI/CD'];
</script>

<Tabs vertical>
  <div slot="tabs">
    {#each tabs as tabName}
      <Tab>{tabName}</Tab>
    {/each}
  </div>

  <div class="pt-2">
    {#each tabs as tabName}
      <TabContent>
        {#each skills.filter((s) => s.type === tabName) as skill}
          <SkillsChip name={skill.label} />
        {/each}
      </TabContent>
    {/each}
  </div>
</Tabs>
