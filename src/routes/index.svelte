<script context="module">
  export const prerender = true;
</script>

<script>
  import { Container, Row, Divider } from 'svelte-materialify';
  import Typewriter from 'svelte-typewriter';
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>
<Container>
  <Row class="d-flex justify-center">
    <h4><strong>Alex So</strong></h4>
  </Row>
  <Row class="d-flex justify-center">
    <Typewriter interval={50}>
      <h6>Passionate in software development and new technologies!</h6>
    </Typewriter>
  </Row>
</Container>
