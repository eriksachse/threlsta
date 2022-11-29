<script>
  import { Canvas } from '@threlte/core';
  import { World } from '@threlte/rapier';
  import Scene from '$lib/Scene.svelte';
</script>

<div class="canvas-wrapper">
  <Canvas>
    <World>
      <Scene />
    </World>
  </Canvas>
</div>

<style>
  .canvas-wrapper {
    position: fixed;
    width: 100%;
    height: 100%;
    background: royalblue;
  }
</style>