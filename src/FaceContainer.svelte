<script>
  export let baseParams;
  const svgHeight = baseParams.svgHeight;
  const svgWidth = baseParams.svgWidth;
  const centerX = svgWidth / 2;
  const centerY = svgHeight / 2;
  const faceStrokeWidth = 10;
  const faceRadius = centerX -4*faceStrokeWidth/2;
  const fillColor = "yellow";
  const strokeColor = "black";
</script>

<style>
</style>

<svg 
  style="
    border: 1px solid black;
    width: {svgWidth}px;
    height: {svgHeight}px;
  ">
  <circle
    r={faceRadius}
    cX={centerX} 
    cY={centerY}
    fill={fillColor} 
    stroke={strokeColor} 
    stroke-width={faceStrokeWidth}
  />
  <g transform={`translate(${centerX},${centerY})`}>
    <slot />
  </g>
</svg>

