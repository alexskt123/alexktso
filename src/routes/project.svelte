<script context="module">
  export const prerender = true;
</script>

<script>
  import { Container, Row, Col } from 'svelte-materialify';
  import Card from '$lib/Card.svelte';
</script>

<svelte:head>
  <title>Projects</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<Container>
  <Row class="d-flex justify-center">
    <Col>
      <Card />
    </Col>
  </Row>
</Container>
