<script>
  import { Chip, Icon } from 'svelte-materialify';
  import { mdiCheckCircleOutline } from '@mdi/js';
  export /**
   * @type {any}
   */
  let name;
</script>

<Chip outlined class="indigo-text ml-1 mt-1">
  <Icon path={mdiCheckCircleOutline} />
  <span>{name}</span>
</Chip>
