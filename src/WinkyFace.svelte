<script>
  import WinkyEyes from './WinkyEyes.svelte';
  import WinkyMouth from './WinkyMouth.svelte';
  export let baseParams;
</script>

<style>
</style>

<WinkyEyes/>
<WinkyMouth svgHeight={baseParams.svgHeight} />

