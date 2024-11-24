<script>
    import { goto } from '$app/navigation';
  </script>
  
  <nav class="bg-gray-800 text-white py-4 px-6">
    <div class="container mx-auto flex justify-between items-center">
      <h1 class="text-2xl font-bold cursor-pointer" on:click={() => goto('/')}>Akash Shop</h1>
      <ul class="flex space-x-4">
        <li class="cursor-pointer hover:text-gray-400" on:click={() => goto('/')}>Home</li>
        <li class="cursor-pointer hover:text-gray-400" on:click={() => goto('/products')}>Products</li>
        <li class="cursor-pointer hover:text-gray-400" on:click={() => goto('/cart')}>Cart</li>
      </ul>
    </div>
  </nav>
  
  <slot />  