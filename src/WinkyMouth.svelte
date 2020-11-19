
<script>
  import {arc} from 'd3-shape';
  export let svgHeight;

  const mouthRadius = svgHeight / 2.9; 
  const mouthStrokeWidth = 10;
  const dimpleRadius = mouthRadius / 4;
  const mouthDimpleAngle = Math.PI / 1.525;  
  const dimpleTransformX = 155;
  const dimpleTransformY = 42;

  const mouthArc = arc()
      .innerRadius(mouthRadius - mouthStrokeWidth)
      .outerRadius(mouthRadius)
      .startAngle(mouthDimpleAngle)
      .endAngle(Math.PI * 3/2);

 const dimpleArc = arc()
      .innerRadius(dimpleRadius - mouthStrokeWidth)
      .outerRadius(dimpleRadius)
      .startAngle(mouthDimpleAngle)
      .endAngle(Math.PI * 3/2);

</script>

<path d={mouthArc()} />
<g transform={`translate(${dimpleTransformX},${dimpleTransformY})`}>
  <path d={dimpleArc()} />
</g>


