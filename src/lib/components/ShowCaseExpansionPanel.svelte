<script>
  // @ts-nocheck

  import { ExpansionPanel } from 'svelte-materialify';

  export /**
   * @type {{ header: any; }}
   */
  let item;
</script>

<ExpansionPanel>
  <span slot="header">
    <strong>{item.header}</strong>
  </span>
  <ul class="mt-5">
    {#each item.listItems as listItem}
      <li class="text--secondary">
        {listItem}
      </li>
    {/each}
  </ul>
</ExpansionPanel>
