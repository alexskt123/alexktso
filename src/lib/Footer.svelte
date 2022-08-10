<script>
  import { isMobile } from 'is-mobile';

  import { Footer, MaterialApp } from 'svelte-materialify';
</script>

<MaterialApp>
  <Footer
    class="blue-grey theme--dark justify-center"
    style={`margin-top:50px;${!isMobile() ? 'padding-left:70px' : ''}`}
  >
    <span>
      Written in <a href="https://kit.svelte.dev">Svelte</a> & Deployed to
      <a href="https://vercel.com">Vercel</a>
    </span>
  </Footer>
</MaterialApp>
