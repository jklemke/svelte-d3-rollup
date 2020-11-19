<script>  
  import SmileyEyes from './SmileyEyes.svelte';
  import SmileyMouth from './SmileyMouth.svelte';
  export let baseParams;
</script>

<style>
</style>

<SmileyEyes />
<SmileyMouth svgHeight={baseParams.svgHeight} />


