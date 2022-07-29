<script>
  import { Chip, Row, Col, MaterialApp } from 'svelte-materialify';
import SkillsChip from './components/SkillsChip.svelte';
</script>

<MaterialApp>
  <Row class="mt-5">
    <SkillsChip name="React.js" />
    <SkillsChip name="Node.js" />
    <SkillsChip name="Next.js" />
    <SkillsChip name="Nest.js" />
    <SkillsChip name="Svelte" />
    <SkillsChip name="Mongo" />
    <SkillsChip name="SQL" />
    <SkillsChip name="Kafka" />
    <SkillsChip name="Java" />
    <SkillsChip name="Progress 4GL" />
  </Row>
</MaterialApp>
