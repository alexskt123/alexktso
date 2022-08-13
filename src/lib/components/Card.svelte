<script>
  import { Card, CardText, Button, Chip, Row, Icon } from 'svelte-materialify';
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

<Row class="d-flex justify-center mt-4 mb-4">
  <Card
    outlined
    style={`padding;min-width:200px;min-height:190px;background-color:${colors.indigo['lighten-5']}`}
  >
    <div class="pt-3 justify-center d-flex">
      <Chip class="theme--dark indigo darken-4">
        <strong>{header}</strong>
      </Chip>
      <a href={link}>
        <Button fab size="x-small" class="ml-1 indigo lighten-1 white-text">
          <Icon path={mdiLinkVariant} />
        </Button>
      </a>
    </div>
    <CardText>
      <strong>{text}</strong>
    </CardText>
  </Card>
</Row>
