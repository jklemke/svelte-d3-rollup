<script>
  import {line} from 'd3-shape';

  const eyeOffsetX = 65;
  const eyeOffsetY = 40;
  const eyeRadius = 35;
  const mouthStrokeWidth = 10;

  let eyeline = line()([[eyeOffsetX - eyeRadius, 0 - eyeOffsetY], [eyeOffsetX + eyeRadius, 0 - eyeOffsetY]]);

</script>


<circle
  cx={-eyeOffsetX}
  cy={-eyeOffsetY}
  r={eyeRadius}
/>

<path d={eyeline} stroke="black" stroke-width={mouthStrokeWidth} fill="none" />        
