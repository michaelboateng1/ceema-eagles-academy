<script>
    import { browser } from '$app/environment';
    
    import { onMount } from 'svelte';
    import 'leaflet/dist/leaflet.css';
    
    import markerIcon2x from 'leaflet/dist/images/marker-icon-2x.png';
    import markerIcon from 'leaflet/dist/images/marker-icon.png';
    import markerShadow from 'leaflet/dist/images/marker-shadow.png';
  
    let mapContainer;
  
    onMount(async () => {
      if(browser){
        const L = await import('leaflet');
        
        delete L.Icon.Default.prototype._getIconUrl;

        L.Icon.Default.mergeOptions({
          iconRetinaUrl: markerIcon2x,
          iconUrl: markerIcon,
          shadowUrl: markerShadow
        });
    
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
      }
    });
  </script>

  <div bind:this={mapContainer} id="map" class="h-[500px] w-full sm:w-[500px] rounded-lg z-0"></div>
  
