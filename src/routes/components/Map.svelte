<script lang="ts">
    import { onMount } from 'svelte';
    import L from 'leaflet';
    import 'leaflet/dist/leaflet.css';
  
    let mapContainer: HTMLDivElement;
  
    onMount(() => {
      const map = L.map(mapContainer).setView([6.636914,  -1.625659], 11);
  
      L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; OpenStreetMap contributors'
      }).addTo(map);
  
      L.marker([6.636914,  -1.625659]).addTo(map)
        .bindPopup('Ceema Eagles Academy', { autoClose: false, closeOnClick: false })
        .openPopup();

      L.marker([6.690425, -1.559298]).addTo(map)
        .bindPopup('SmartTribe', { autoClose: false, closeOnClick: false })
        .openPopup();
    });
  </script>

  <div bind:this={mapContainer} id="map" class="h-[500px] w-full sm:w-[500px] rounded-lg z-0"></div>
  

  
  