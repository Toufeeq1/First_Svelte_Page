<script>
    let mousePosition = { x: 0, y: 0 };
  
    const handleMouseMove = (e) => {
      mousePosition = { x: e.clientX, y: e.clientY };
    };
  </script>
  
  <style>
   h1{
    color:#FF3E00;
   }
  </style>
  
  
  <svelte:window on:mousemove={handleMouseMove} />

  <h1>The mouse position is at x:{mousePosition.x} y:{mousePosition.y}</h1>
  
  