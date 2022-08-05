<script context="module">
  export const prerender = true;
</script>

<script>
  import { Container, Row } from 'svelte-materialify';
  import Experience from '$lib/Experience.svelte';
  import Skills from '$lib/Skills.svelte';
  import Footer from '$lib/Footer.svelte';
  import Education from '$lib/Education.svelte';
  import Sharing from '$lib/Sharing.svelte';
  import CustomTypeWrite from '$lib/components/CustomTypeWrite.svelte';
  import PersonalProjects from '$lib/PersonalProjects.svelte';
  import SectionHeader from '$lib/components/SectionHeader.svelte';
</script>

<svelte:head>
  <title>Alex's Profile</title>
  <meta name="description" content="alexktso Profile App" />
</svelte:head>
<Container style="padding-left:70px">
  <Row class="d-flex justify-center text-center mt-10">
    <h4><strong>Alex So</strong></h4>
  </Row>
  <Row class="d-flex justify-center text-center pt-2">
    <CustomTypeWrite />
  </Row>
  <Row class="d-flex justify-center text-center pt-2">
    <Sharing />
  </Row>
  <SectionHeader headerName={'Work Experience'} />
  <Experience />
  <SectionHeader headerName={'Education'} />
  <Education />
  <SectionHeader headerName={'My Personal Projects'} />
  <PersonalProjects />
  <SectionHeader headerName={'Skills'} />
  <Skills />
</Container>
<Footer />
