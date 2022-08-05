<script>
  import { Card, CardText, Button, MaterialApp, Chip, Row, Icon } from 'svelte-materialify';
  import { mdiLinkVariant } from '@mdi/js';
  import colors from 'svelte-materialify/src/utils/colors';
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
    <Card
      outlined
      class="backg"
      style={`min-width:200px;max-width:300px;min-height:190px;background-color:${colors.lightBlue['lighten-5']}`}
    >
      <div class="pl-4 pr-4 pt-3">
        <Chip class="theme--dark cyan darken-4">
          <strong>{header}</strong>
        </Chip>
        <a href={link}>
          <Button fab size="x-small" class="blue white-text">
            <Icon path={mdiLinkVariant} />
          </Button>
        </a>
      </div>
      <CardText>
        <strong>{text}</strong>
      </CardText>
    </Card>
  </Row>
</MaterialApp>
