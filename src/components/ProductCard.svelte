<script>
    export let product;
  </script>
  
  <div class="border rounded-lg p-4 shadow hover:shadow-lg">
    <img src={product.image} alt={product.name} class="w-full h-48 object-cover rounded" />
    <h2 class="text-lg font-bold mt-2">{product.name}</h2>
    <p class="text-blue-600 font-bold">₹{product.price}</p>
    <button class="bg-green-500 text-white px-4 py-2 rounded mt-2 hover:bg-blue-700">
      Add to Cart
    </button>
  </div>  