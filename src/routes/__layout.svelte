<script>
  import { Container, Row, Col } from 'svelte-materialify';
  import Drawer from '$lib/Drawer.svelte';
  import Footer from '$lib/Footer.svelte';
  import '../app.css';
</script>

<!-- <Header /> -->
<Container>
  <Row>
    <Col cols={2} lg={1}>
      <Drawer />
    </Col>
    <Col>
      <slot />
    </Col>
  </Row>
</Container>

<Footer />
