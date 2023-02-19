<script>
  import { onMount } from 'svelte';
  import { createEventDispatcher } from 'svelte';
  const dispatch = createEventDispatcher();

  //import mapStyles from './map-styles'; // optional

  export let globally = false;
  export let map;

  let src = '';
  const key = 'AIzaSyD_Y04wxTKvDDJrmqGDoIo8D4EGUWe37B8'; 

  // @ts-ignore
  let container;
  let zoom = 13;
  let center = { lat: 39.726723, lng: -75.2620343 };

  onMount(() => {
      Object.assign(window, {
          mapLoaded: () => {
              // @ts-ignore
              map = new google.maps.Map(container, {
                  zoom,
                  center
                  // styles: mapStyles
              });
              dispatch('load', true);
              if (globally) {
                  Object.assign(window, { map });
              }
          }
      });

      //Assign
      src = `https://maps.googleapis.com/maps/api/js?key=${key}&callback=mapLoaded`;
  });
</script>

<!-- This is tailwind css class change with whatever fits to your case. -->
<div class="map w-full h-full" bind:this={container} />
<svelte:head>
  {#if src}
      <script {src}></script>
  {/if}
</svelte:head>


<location
 {map}
 globally
 on:load={() => {
  console.log('MAP SAYS IM LOADED');
 }}
/>
