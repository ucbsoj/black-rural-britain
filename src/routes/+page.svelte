<script lang="ts">
  import rawBlocks from '$lib/doc.blocks.json';
  import DocRenderer from '$lib/components/DocRenderer.svelte';
  import type { Block } from '$lib/components/DocRenderer.svelte';
  const blocks = rawBlocks as Block[];
</script>



<!-- 
Hard-code custom code that should appear BEFORE Google Doc here. 
This code is in +page.svelte and can be manually coded using HTML or Svelte tags.
-->
<header class="container-fluid d-flex flex-column align-items-center justify-content-center vh-100" style="background-image:url('hero.jpg');background-size:cover;background-position:center;">
  <h1 class="text-start ps-0 ps-sm-5 display-1 pinyon w-100">
    <span class="d-block">Black</span> 
    <span class="d-block ps-0 ps-sm-2">Rural</span> 
    <span class="d-block ps-0 ps-sm-4">Britain</span>
  </h1>
</header>


<section class="container-fluid bg-black vh-75 d-flex flex-column">
  <!-- Top ornamental strip -->
  <div class="container-fluid align-self-start" style="background-image:url('ornaments.png');background-repeat:repeat-x;background-size:contain;height:0;padding-bottom:8%;">
    <p>&nbsp;</p>
  </div>

  <div class="container-fluid bg-black d-flex flex-column align-items-center justify-content-center align-self-center my-auto">
    <div class="row justify-content-center">
      <figure class="col-12 col-sm-10 col-md-8">
        <blockquote class="blockquote text-white text-start text-sm-center">
          <p class="crimson fs-1">&ldquo;As Black people , we might feel that the countryside is not for us, but who said that?&rdquo;</p>
        </blockquote>
        <figcaption class="blockquote-footer text-start text-sm-center fs-4 mt-3">
          <p>Flavian Obiero</p>
        </figcaption>
      </figure>
    </div>
  </div>

  <!-- Bottom ornamental strip -->
  <div class="container-fluid align-self-end" style="background-image:url('ornaments.png');background-repeat:repeat-x;background-size:contain;height:0;padding-bottom:8%;">
    <p>&nbsp;</p>
  </div>
</section>

<div class="container-fluid vh-50 d-flex flex-column align-items-center justify-content-center" style="background-image:url('boats.jpg');background-size:cover;background-position:center;">
  <h2 class="crimson display-2" style="letter-spacing:0.3rem">Staking a Claim</h2>
</div>


<!-- DO NOT EDIT (except to modify classes). This will become code imported from Google Doc. -->
<div class="container mt-5">
  <div class="row justify-content-center">
    <div class="col-12 col-sm-10 col-lg-8 col-xxl-6">
      <DocRenderer {blocks} />
    </div>
  </div>
</div>


<!-- Hard-code any custom code that should appear AFTER Google Doc below here. -->
<footer class="container-fluid bg-dark text-white p-5">
  <p class="text-center">See template on <a class="text-white" href="https://github.com/jrue/multimedia-template-2026" target="_blank">Github</a></p>
</footer>