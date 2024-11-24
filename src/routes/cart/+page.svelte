<script>
    import Navbar from '../../components/Navbar.svelte';
  
    let cartItems = [
      { id: 1, name: 'Product A', price: 500 },
      { id: 2, name: 'Product B', price: 700 },
    ];
  </script>
  
  <Navbar />
  
  <div class="container mx-auto p-4">
    <h1 class="text-2xl font-bold mb-4">Your Cart</h1>
    <ul>
      {#each cartItems as item}
        <li class="flex justify-between border-b py-2">
          <span>{item.name}</span>
          <span>₹{item.price}</span>
        </li>
      {/each}
    </ul>
    <p class="mt-4 text-lg font-bold">
      Total: ₹{cartItems.reduce((total, item) => total + item.price, 0)}
    </p>
  </div>  