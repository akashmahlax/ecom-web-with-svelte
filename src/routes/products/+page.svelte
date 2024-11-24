<script>
    import Navbar from '../../components/Navbar.svelte';
    import ProductCard from '../../components/ProductCard.svelte';
  
    let products = [
      { id: 1, name: 'asla', price: 500, image: 'https://via.placeholder.com/150' },
      { id: 2, name: 'toffia', price: 700, image: 'https://via.placeholder.com/150' },
      { id: 3, name: 'jalebi', price: 300, image: 'https://via.placeholder.com/150' },
    ];
  </script>
  
  <Navbar />
  
  <div class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-6 p-4">
    {#each products as product}
      <ProductCard {product} />
    {/each}
  </div>  