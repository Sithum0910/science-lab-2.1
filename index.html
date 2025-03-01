<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>3D Gravity Simulation</title>
  <style>
    body {
      margin: 0;
      overflow: hidden;
      font-family: Arial, sans-serif;
    }
    #info {
      position: absolute;
      top: 20px;
      left: 20px;
      color: white;
      font-size: 18px;
    }
  </style>
</head>
<body>
  <div id="info">Developed by Sithum | <a href="https://github.com/Sithum0910" target="_blank" style="color: #6e5494;">GitHub</a></div>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r146/three.min.js"></script>
  <script>
    // Scene, Camera, Renderer
    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    const renderer = new THREE.WebGLRenderer();
    renderer.setSize(window.innerWidth, window.innerHeight);
    document.body.appendChild(renderer.domElement);

    // Lighting
    const light = new THREE.DirectionalLight(0xffffff, 1);
    light.position.set(5, 5, 5).normalize();
    scene.add(light);

    // Earth (Sphere)
    const earthGeometry = new THREE.SphereGeometry(1, 32, 32);
    const earthMaterial = new THREE.MeshPhongMaterial({ color: 0x0000ff });
    const earth = new THREE.Mesh(earthGeometry, earthMaterial);
    scene.add(earth);

    // Moon (Sphere)
    const moonGeometry = new THREE.SphereGeometry(0.2, 32, 32);
    const moonMaterial = new THREE.MeshPhongMaterial({ color: 0xaaaaaa });
    const moon = new THREE.Mesh(moonGeometry, moonMaterial);
    moon.position.set(3, 0, 0); // Start 3 units away from Earth
    scene.add(moon);

    // Variables for Gravity Simulation
    const G = 0.1; // Gravitational constant (custom value for simulation)
    const earthMass = 100; // Mass of Earth
    const moonMass = 1; // Mass of Moon
    let moonVelocity = new THREE.Vector3(0, 0.5, 0); // Initial velocity of the Moon

    // Animation Loop
    function animate() {
      requestAnimationFrame(animate);

      // Calculate gravitational force
      const distanceVector = new THREE.Vector3().subVectors(earth.position, moon.position);
      const distance = distanceVector.length();
      const forceMagnitude = (G * earthMass * moonMass) / (distance * distance);
      const force = distanceVector.normalize().multiplyScalar(forceMagnitude);

      // Update Moon's velocity and position
      moonVelocity.add(force.multiplyScalar(0.01)); // Small time step for stability
      moon.position.add(moonVelocity);

      // Render the scene
      renderer.render(scene, camera);
    }

    // Camera Position
    camera.position.z = 5;

    // Handle Window Resize
    window.addEventListener('resize', () => {
      camera.aspect = window.innerWidth / window.innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(window.innerWidth, window.innerHeight);
    });

    // Start Animation
    animate();
  </script>
</body>
</html>
