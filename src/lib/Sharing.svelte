<script>
  import { Button, Icon, MaterialApp } from 'svelte-materialify';
  import { mdiApps, mdiGithub, mdiLinkedin } from '@mdi/js';
</script>

<MaterialApp>
  <a href="/about">
    <Button fab>
      <Icon path={mdiApps} />
    </Button>
  </a>
  <a href="https://github.com/alexskt123">
    <Button fab class="black white-text">
      <Icon path={mdiGithub} />
    </Button>
  </a>
  <a href="https://www.linkedin.com/in/alex-so-724135147/">
    <Button fab class="blue white-text">
      <Icon path={mdiLinkedin} />
    </Button>
  </a>
</MaterialApp>
