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

  let mini = true;
  function mouseEnter() {
    mini = false;
  }
  function mouseLeave() {
    mini = true;
  }
</script>

<MaterialApp>
  <div class="d-inline-block" on:mouseenter={mouseEnter} on:mouseleave={mouseLeave}>
    <NavigationDrawer absolute left {mini}>
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
        <a sveltekit:prefetch href="/project" on:click={mouseLeave}>
          <ListItem active={$page.url.pathname === '/project'}>
            <span slot="prepend">
              <Icon path={mdiListBoxOutline} />
            </span>
            Projects
          </ListItem>
        </a>
      </List>
    </NavigationDrawer>
  </div>
</MaterialApp>
