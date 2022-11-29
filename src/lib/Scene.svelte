<script>
  import { T, useFrame, OrbitControls } from '@threlte/core';
  let r = 0;

  useFrame((_, delta) => {
    r += 0.5 * delta;
  })
</script>

<T.PerspectiveCamera makeDefault position.y={5} position.z={10}>
  <OrbitControls />
</T.PerspectiveCamera>

<T.DirectionalLight />
<T.AmbientLight />

<T.Mesh rotation.x={r} rotation.y={r}>
  <T.IcosahedronGeometry />
  <T.MeshStandardMaterial color={'coral'} />
</T.Mesh>

<T.GridHelper />