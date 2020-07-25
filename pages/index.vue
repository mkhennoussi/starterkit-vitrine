<template>
  <div class="antialiased leading-normal min-h-full">
    <Navbar />
    <div class="bg-white z-10 relative">
      <div
        class="container mx-auto grid  grid-cols-1 md:grid-cols-2 gap-0 py-8 md:p-0 md:mt-32">
        <div class="flex justify-center flex-wrap items-center ">
          <div>
            <Logo class="h-32" />
          </div>
          <h1
            class="font-bold w-full text-center text-gray-900 uppercase text-4xl  tracking-wider">
            AB PERMIS</h1>
          <p
            class="block  text-gray-600 text-center w-5/6 py-4  md:w-2/3">
            Découvrez
            l'auto école qui
            vous accompagnera
            pour réussir du premier coup !</p>
        </div>
        <div class="flex justify-center items-center">
          <!-- <img class="card-image rounded shadow-lg "
            src="https://images.pexels.com/photos/919073/pexels-photo-919073.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500"
            alt=""> -->
          <img src="~/assets/images/c3.jpg" />
        </div>
      </div>
    </div>
    <svg class="md:-mt-32 z-10 fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill-opacity="1"
        d="M0,96L240,224L480,256L720,192L960,256L1200,288L1440,64L1440,320L1200,320L960,320L720,320L480,320L240,320L0,320Z">
      </path>
    </svg>
    <!-- <svg class="fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill-opacity="1"
        d="M0,288L720,96L1440,224L1440,320L720,320L0,320Z"></path>
    </svg> -->
    <!-- <svg class="fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill-opacity="1"
        d="M0,224L480,64L960,160L1440,32L1440,320L960,320L480,320L0,320Z">
      </path>
    </svg> -->
    <!-- <svg class="bg-red-400 fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill-opacity="1"
        d="M0,64L720,192L1440,192L1440,320L720,320L0,320Z"></path>
    </svg> -->
    <div class="md:-mt-8 bg-gray-100">
      <div class="py-8">
        <div class="container mx-auto px-2 md:px-8">
          <h1
            class="font-bold uppercase text-5xl text-primary-500 m-8 px-2 md:px-0 text-center">
            NOS OFFRES</h1>
          <div
            class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-2 pb-8">
            <service-card v-for="(item, index) in offers" :key="index"
              :title="item.title" :description="item.description">
              <svg class="fill-current h-12" viewBox="0 0 20 20">
                <path
                  d="M18 2c-.5-.6-1 0-3 .8-5 2.5-13.9 7.4-13.9 7.4l7.6 1.1 1 7.6s5-8.8 7.5-14c.9-1.8 1.4-2.4.9-3zm-1.8 1.9l-5.5 10.2-.5-4.6 6-5.6z" />
              </svg>
            </service-card>
          </div>
        </div>
      </div>
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill="#F7FAFC" fill-opacity="1"
        d="M0,128L288,160L576,64L864,32L1152,96L1440,32L1440,0L1152,0L864,0L576,0L288,0L0,0Z">
      </path>
    </svg>
    <div class="footer container mx-auto">
      <div
        class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-2 pb-8">
        <Logo class="h-48" />
        <div class="text-center md:text-left flex flex-col">
          <h2 class="text-lg text-primary-500 ">AB PERMIS</h2>
          <div class="text-gray-500">contact@abpermis.com
          </div>
          <div class="text-gray-600">06-83-38-19-16</div>
        </div>

      </div>
    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      offers: [
        {
          title: "Permis B",
          description: "Obtenez votre permis B rapidement et facilement",
          price: "998€"
        },
        {
          title: "Conduite accompagnée",
          description: "Débutez dès 16 ans la conduite afin d'être au top le jour du permis",
          price: "1238€"
        },
        {
          title: "Permis Deux roues",
          description: "Vous êtes plûtot 2 roues, passez le permis !",
          price: "1238€"
        },
      ]
    }
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.card-image {
  transform: perspective(200px) rotateY(-2deg);
}
</style>
