<script context="module">
  export const prerender = true;
</script>

<script>
  import { Container, Row, Col } from 'svelte-materialify';
  import Typewriter from 'svelte-typewriter';
  import Card from '$lib/Card.svelte';
  import Experience from '$lib/Experience.svelte';
  import Skills from '$lib/Skills.svelte';
  import Footer from '$lib/Footer.svelte';
  import Education from '$lib/Education.svelte';
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="alexktso Profile App" />
</svelte:head>
<Container style="padding-left:70px">
  <Row class="d-flex justify-center text-center">
    <h5><strong>Alex So</strong></h5>
  </Row>
  <Row class="d-flex justify-center text-center pt-5">
    <Typewriter interval={50}>
      <h6>Passionate in software development and new technologies!</h6>
    </Typewriter>
  </Row>
  <Row class="d-flex justify-center text-center pt-15">
    <h5><strong>My Personal Projects</strong></h5>
  </Row>
  <Row class="d-flex justify-center">
    <Col class="ml-1 mr-1">
      <Card
        header={'Stock Is Fun'}
        text={'A website built with Nextjs and Firebase to study Stock'}
        link={'https://stockisfun.vercel.app'}
      />
    </Col>
    <Col class="ml-1 mr-1">
      <Card
        header={'Share Text'}
        text={'A website built with Material UI, Nextjs and Firebase for text sharing'}
        link={'https://share-text-fast.vercel.app'}
      />
    </Col>
    <Col class="ml-1 mr-1">
      <Card
        header={'Profile'}
        text={'A website built with Svelte to display my personal profile'}
        link={'https://alexktso.vercel.app'}
      />
    </Col>
    <Col class="ml-1 mr-1">
      <Card
        header={'Excel-ERD'}
        text={'A transformer program to draw ER diagrams with input excel file, using Node.js and PlantUML'}
        link={'https://github.com/alexskt123/excel-to-erd'}
      />
    </Col>
  </Row>
  <Row class="d-flex justify-center text-center pt-15">
    <h5><strong>Work Experience</strong></h5>
  </Row>
  <Experience />
  <Row class="d-flex justify-center text-center pt-15">
    <h5><strong>Education</strong></h5>
  </Row>
  <Education />
  <Row class="d-flex justify-center text-center pt-15">
    <h5><strong>Skills</strong></h5>
  </Row>
  <Skills />
</Container>
<Footer />
