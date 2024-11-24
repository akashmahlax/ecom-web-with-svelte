<script>
  import Navbar from '../../components/Navbar.svelte';
  import Footer from '../../components/Footer.svelte';
  import ProductCard from '../../components/ProductCard.svelte';

  let products = [
    { id: 1, name: 'Product A', price: 500, image: 'https://via.placeholder.com/300' },
    { id: 2, name: 'Product B', price: 700, image: 'https://via.placeholder.com/300' },
    { id: 3, name: 'Product C', price: 300, image: 'https://via.placeholder.com/300' },
  ];
</script>

<Navbar />

<div class="container mx-auto p-4">
  <h1 class="text-3xl font-bold mb-6">Our Products</h1>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each products as product}
      <ProductCard {product} />
    {/each}
  </div>
</div>

<Footer />