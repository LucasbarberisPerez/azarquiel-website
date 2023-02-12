<script>
    import {slide} from 'svelte/transition';
  </script>
  
    <div
      transition:slide="{{ y: -50, duration: 2500, delay: 300 }}">
      <slot/>
    </div>