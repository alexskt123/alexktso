<script context="module">
  export const prerender = true;
</script>

<script>
  import { Row, Col } from 'svelte-materialify';
  import Card from '$lib/components/Card.svelte';
  import { personalProjects } from './config';
</script>

<Row class="d-flex justify-center">
  {#each personalProjects as personalProject}
    <Col class="ml-1 mr-1">
      <Card {...personalProject} />
    </Col>
  {/each}
</Row>
