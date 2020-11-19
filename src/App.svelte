<script>
  import FaceContainer from "./FaceContainer.svelte";
  import SmileyFace from "./SmileyFace.svelte";
  import WinkyFace from "./WinkyFace.svelte";

  const baseParams = {
    svgHeight: 480,
    svgWidth: 480
  }
</script>

<style>  
</style>

<h1>Smiley Face and Winky Face built with rollup, svelte, svg, and d3</h1>
<div>
  <FaceContainer {baseParams} >
    <SmileyFace {baseParams} />  
  </FaceContainer>
  <FaceContainer {baseParams} >
    <WinkyFace {baseParams}/>  
  </FaceContainer>
</div>

