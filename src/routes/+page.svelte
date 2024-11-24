<script>
  import Navbar from '../components/Navbar.svelte';
  import Footer from '../components/Footer.svelte';
  import Testimonials from '../components/Testimonials.svelte';
</script>

<Navbar />

<div class="bg-gradient-to-br from-blue-500 to-green-500 text-white py-20 text-center">
  <h1 class="text-6xl font-bold">Welcome to akash Shop</h1>
  <p class="mt-4 text-xl">Your one-stop shop for quality products</p>
  <button
    class="mt-6 bg-white text-blue-600 py-3 px-8 rounded-lg shadow-lg hover:bg-gray-100"
    on:click={() => goto('/products')}>
    Shop Now
  </button>
</div>

<section class="container mx-auto mt-10">
  <h2 class="text-4xl font-bold text-center">Why Choose Us?</h2>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-6">
    <div class="p-6 bg-white rounded shadow hover:shadow-lg text-center">
      <h3 class="text-2xl font-bold mb-2">High Quality</h3>
      <p>Our products are handpicked for excellence.</p>
    </div>
    <div class="p-6 bg-white rounded shadow hover:shadow-lg text-center">
      <h3 class="text-2xl font-bold mb-2">Affordable Prices</h3>
      <p>Get the best deals without breaking the bank.</p>
    </div>
    <div class="p-6 bg-white rounded shadow hover:shadow-lg text-center">
      <h3 class="text-2xl font-bold mb-2">Fast Delivery</h3>
      <p>Receive your products in record time.</p>
    </div>
  </div>
</section>



<Footer />