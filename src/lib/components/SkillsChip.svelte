<script>
  import { Col, Chip, MaterialApp, Icon } from 'svelte-materialify';
  import { mdiCheckCircleOutline } from '@mdi/js';
  export /**
   * @type {any}
   */
  let name;
</script>

<MaterialApp>
  <Col class="ml-1">
    <Chip outlined class="indigo-text">
      <Icon path={mdiCheckCircleOutline} />
      <span>{name}</span>
    </Chip>
  </Col>
</MaterialApp>
