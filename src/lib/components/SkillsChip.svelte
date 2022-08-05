<script>
  import { Col, Chip, MaterialApp, Icon } from 'svelte-materialify';
  import { mdiCheckCircleOutline } from '@mdi/js';
  export /**
   * @type {any}
   */
  let name;
</script>

<MaterialApp>
  <Col class="ml-1" style="padding: 0.1rem">
    <Chip outlined class="indigo-text" style="min-width:200px">
      <Icon path={mdiCheckCircleOutline} />
      <span>{name}</span>
    </Chip>
  </Col>
</MaterialApp>
