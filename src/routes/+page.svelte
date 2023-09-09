<script>
  import "../app.css";
  import { onMount } from "svelte";
  import vCard from "vcf";
  let contactData;


  onMount(() => {
    const link = document.createElement('a');
    link.href = '/Okita_Stephen.vcf';
    link.download = 'Okita_Stephen.vcf';
    document.body.appendChild(link);
    link.click();
    document.body.removeChild(link);
  });
</script>

<!-- <button on:click={saveFile}>Save File</button> -->
<div style="display: flex; justify-content: center; align-items: center; height: 100vh;">
  <a href="/Okita_Stephen.vcf" download> Save Contact</a>
</div>
  <!-- Display other relevant contact information -->

<style>
 a{
    background-color: var(--purple);
    padding: 2rem;
 }
</style>