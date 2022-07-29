<script>
  import { Card, CardText, Button, MaterialApp, Chip, Row, Icon } from 'svelte-materialify';
  import { mdiLinkVariant } from '@mdi/js';
  export /**
   * @type {any}
   */
  let header;
  export /**
   * @type {any}
   */
  let text;
  export /**
   * @type {any}
   */
  let link;
</script>

<MaterialApp>
  <Row class="d-flex justify-center mt-4 mb-4">
    <Card outlined style="min-width:200px;max-width:300px;min-height:200px;">
      <div class="pl-4 pr-4 pt-3">
        <Chip class="teal lighten-5">
          <strong>{header}</strong>
        </Chip>
        <a href={link}>
          <Button fab size="x-small" class="blue white-text">
            <Icon path={mdiLinkVariant} />
          </Button>
        </a>
      </div>
      <CardText>
        {text}
      </CardText>
    </Card>
  </Row>
</MaterialApp>
