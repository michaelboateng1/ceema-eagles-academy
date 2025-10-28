<script lang="ts">
    import { onMount } from 'svelte';
    import L from 'leaflet';
    import 'leaflet/dist/leaflet.css';
  
    let mapContainer: HTMLDivElement;
  
    onMount(() => {
      const map = L.map(mapContainer).setView([5.6037, -0.1870], 13); // Accra, Ghana
  
      L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; OpenStreetMap contributors'
      }).addTo(map);
  
      L.marker([5.6037, -0.1870]).addTo(map)
        .bindPopup('Ceema Eagles Academy')
        .openPopup();

      L.marker([6.6037, -0.2870]).addTo(map)
        .bindPopup('Hello from SmartTribe')
        // .openPopup();
    });
  </script>

  <div bind:this={mapContainer} id="map" class="h-[500px] w-[500px] z-0"></div>
  

  
  