<script>
    import Navbar from '../components/Navbar.svelte';
    import Footer from '../components/Footer.svelte';
  
    let testimonials = [
      {
        name: 'John Doe',
        role: 'Software Engineer',
        image: 'https://via.placeholder.com/150',
        feedback:
          'This e-commerce site is fantastic! The user interface is smooth and easy to navigate. Highly recommended.',
      },
      {
        name: 'Jane Smith',
        role: 'Digital Marketer',
        image: 'https://via.placeholder.com/150',
        feedback:
          'I found everything I needed in one place. Customer service was excellent, and the products are top-notch!',
      },
      {
        name: 'Michael Johnson',
        role: 'Entrepreneur',
        image: 'https://via.placeholder.com/150',
        feedback:
          'Absolutely loved the experience. The checkout process was seamless, and the delivery was prompt.',
      },
    ];
  </script>
  
  <Navbar />
  
  <div class="container mx-auto px-4 py-10">
    <h1 class="text-4xl font-bold text-center mb-8">Testimonials</h1>
    <p class="text-center text-gray-600 mb-12">
      Hear what our customers are saying about us.
    </p>
  
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      {#each testimonials as testimonial}
        <div class="bg-white shadow-md rounded-lg p-6">
          <div class="flex items-center mb-4">
            <img
              class="w-16 h-16 rounded-full mr-4"
              src={testimonial.image}
              alt="{testimonial.name}"
            />
            <div>
              <h3 class="text-lg font-bold">{testimonial.name}</h3>
              <p class="text-sm text-gray-500">{testimonial.role}</p>
            </div>
          </div>
          <p class="text-gray-700">"{testimonial.feedback}"</p>
        </div>
      {/each}
    </div>
  </div>
  
  <Footer />  