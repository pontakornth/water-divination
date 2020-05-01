<script>
import { onMount } from 'svelte';
let canvas;
let width = 800;
let height = 800;

onMount(() => {
    const ctx = canvas.getContext('2d');

    //Draw water
    ctx.beginPath();
    ctx.fillStyle = 'skyblue';
    ctx.arc(width / 2,height / 2,200,0,Math.PI * 2);
    ctx.fill();
    

    //Draw aura
    ctx.beginPath();
    ctx.strokeStyle = 'skyblue';
    ctx.arc(width / 2,height / 2,250,0,Math.PI * 2);
    ctx.stroke();

    //Draw rect
    ctx.beginPath();
    ctx.fillStyle = 'lightgreen';
    ctx.rect(width / 2 - 50, height / 2 - 50,100,100);
    ctx.fill();
    
})

</script>

<canvas 
  bind:this={canvas} 
  width="800"
  height="800"
/>