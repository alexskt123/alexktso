<script>
  import {
    NavigationDrawer,
    List,
    ListItem,
    Avatar,
    Divider,
    Icon,
    MaterialApp
  } from 'svelte-materialify';
  import { mdiHomeCity, mdiListBoxOutline } from '@mdi/js';
  import { page } from '$app/stores';
  import colors from 'svelte-materialify/src/utils/colors';

  let mini = true;
  function mouseEnter() {
    mini = false;
  }
  function mouseLeave() {
    mini = true;
  }
</script>

<MaterialApp>
  <div on:mouseenter={mouseEnter} on:mouseleave={mouseLeave}>
    <NavigationDrawer
      class="theme--dark"
      fixed
      {mini}
      style={`background-color:${colors.blueGrey['darken-3']}`}
    >
      <ListItem>
        <span slot="prepend" class="ml-n2">
          <Avatar size={40}><img src="/profile.jpeg" alt="profile" /></Avatar>
        </span>
        <strong>Alex So</strong>
      </ListItem>
      <Divider />
      <List dense nav>
        <a sveltekit:prefetch href="/" on:click={mouseLeave}>
          <ListItem active={$page.url.pathname === '/'}>
            <span slot="prepend">
              <Icon path={mdiHomeCity} />
            </span>
            Home
          </ListItem>
        </a>
        <a sveltekit:prefetch href="/about" on:click={mouseLeave}>
          <ListItem active={$page.url.pathname === '/about'}>
            <span slot="prepend">
              <Icon path={mdiListBoxOutline} />
            </span>
            About
          </ListItem>
        </a>
      </List>
    </NavigationDrawer>
  </div>
</MaterialApp>
