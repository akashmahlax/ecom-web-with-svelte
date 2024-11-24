<script>
  import { goto } from '$app/navigation';
</script>

<nav class="bg-blue-600 text-white py-4 px-6 shadow-lg">
  <div class="container mx-auto flex justify-between items-center">
    <h1 class="text-2xl font-bold cursor-pointer" on:click={() => goto('/')}>
      akashShop
    </h1>
    <ul class="flex space-x-6">
      <li class="hover:underline cursor-pointer" on:click={() => goto('/')}>
        Home
      </li>
      <li class="hover:underline cursor-pointer" on:click={() => goto('/products')}>
        Products
      </li>
      <li class="hover:underline cursor-pointer" on:click={() => goto('/cart')}>
        Cart
      </li>
      <li class="hover:underline cursor-pointer" on:click={() => goto('/contact')}>
        Contact
      </li>
    </ul>
  </div>
</nav>