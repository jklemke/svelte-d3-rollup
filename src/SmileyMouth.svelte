
<script>
  import {arc} from 'd3-shape';
  export let svgHeight;
  const mouthRadius = svgHeight / 2.9; 
  const mouthStrokeWidth = 10;

  const mouthArc = arc()
      .innerRadius(mouthRadius - mouthStrokeWidth)
      .outerRadius(mouthRadius)
      .startAngle(Math.PI / 2)
      .endAngle(Math.PI * 3/2);

</script>

<path d={mouthArc()} />


