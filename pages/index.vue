<template>
  <div class="antialiased leading-normal min-h-full text-gray-900">
    <Navbar />
    <div class="bg-white z-10 relative">
      <div class="container mx-auto grid grid-cols-1 md:grid-cols-2 gap-0 py-8 md:p-0 md:mt-32">
        <div class="flex justify-center flex-wrap items-center">
          <div>
            <Logo class="h-48" />
          </div>
          <h1
            class="font-bold w-full text-center text-gray-900 uppercase text-4xl tracking-wider"
          >AB PERMIS</h1>
          <p class="block text-gray-600 text-center w-5/6 py-4 md:w-2/3">
            Découvrez
            l'auto école qui
            vous accompagnera
            pour réussir du premier coup !
          </p>
        </div>
        <div class="flex justify-center items-center">
          <!-- <img class="card-image rounded shadow-lg "
            src="https://images.pexels.com/photos/919073/pexels-photo-919073.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500"
          alt="">-->
          <img src="~/assets/images/c3-2020.jpg" />
        </div>
      </div>
    </div>
    <svg
      class="md:-mt-32 z-10 fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 1440 320"
    >
      <path
        fill-opacity="1"
        d="M0,96L240,224L480,256L720,192L960,256L1200,288L1440,64L1440,320L1200,320L960,320L720,320L480,320L240,320L0,320Z"
      />
    </svg>

    <div class="md:-mt-8 bg-gray-100">
      <div class="py-8 px-4">
        <div class="container mx-auto">
          <h1
            class="font-bold uppercase text-5xl md:text-6xl text-gray-900 md:mb-16 leading-none mb-8 px-2 md:px-0 text-center"
          >Code de la route</h1>
          <div
            class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-12 pb-8"
          >
            <service-card
              v-for="(item, index) in offersOther"
              :key="index"
              :title="item.title"
              :description="item.description"
              :price="item.price"
            >
              <svg class="fill-current h-12" viewBox="0 0 20 20">
                <path
                  d="M18 2c-.5-.6-1 0-3 .8-5 2.5-13.9 7.4-13.9 7.4l7.6 1.1 1 7.6s5-8.8 7.5-14c.9-1.8 1.4-2.4.9-3zm-1.8 1.9l-5.5 10.2-.5-4.6 6-5.6z"
                />
              </svg>
            </service-card>
          </div>
        </div>
      </div>

      <div class="py-8 px-4">
        <div class="container mx-auto">
          <h1
            class="font-bold uppercase text-5xl md:text-6xl text-gray-900 md:mb-16 m-8 px-2 md:px-0 text-center leading-none"
          >NOS OFFRES AUTO</h1>
          <div
            class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-12 pb-8"
          >
            <service-card
              v-for="(item, index) in offersAuto"
              :key="index"
              :title="item.title"
              :description="item.description"
              :price="item.price"
            >
              <svg class="fill-current h-12" viewBox="0 0 20 20">
                <path
                  d="M18 2c-.5-.6-1 0-3 .8-5 2.5-13.9 7.4-13.9 7.4l7.6 1.1 1 7.6s5-8.8 7.5-14c.9-1.8 1.4-2.4.9-3zm-1.8 1.9l-5.5 10.2-.5-4.6 6-5.6z"
                />
              </svg>
            </service-card>
          </div>
        </div>
      </div>

      <div class="py-8 px-4">
        <div class="container mx-auto">
          <h1
            class="font-bold uppercase text-5xl md:text-6xl text-gray-900 md:mb-16 m-8 px-2 md:px-0 leading-none text-center"
          >NOS OFFRES MOTO</h1>
          <div
            class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-12 pb-8"
          >
            <service-card
              v-for="(item, index) in offersMoto"
              :key="index"
              :title="item.title"
              :description="item.description"
              :price="item.price"
            >
              <svg class="fill-current h-12" viewBox="0 0 20 20">
                <path
                  d="M18 2c-.5-.6-1 0-3 .8-5 2.5-13.9 7.4-13.9 7.4l7.6 1.1 1 7.6s5-8.8 7.5-14c.9-1.8 1.4-2.4.9-3zm-1.8 1.9l-5.5 10.2-.5-4.6 6-5.6z"
                />
              </svg>
            </service-card>
          </div>
        </div>
      </div>

      <div class="py-8 px-4">
        <div class="container mx-auto">
          <h1
            class="font-bold uppercase text-4xl md:text-6xl text-gray-900 m-8 mb-16 px-2 md:px-0 text-center"
          >Documents à fournir</h1>
          <div
            class="bg-white p-12 flex flex-col items-center justify-center shadow-md rounded-2xl md:rounded-3xl"
          >
            <p class="text-gray-900 text-lg">
              Pour vous compter parmis
              notre équipe de super-conducteur, veuillez nous envoyez
              par email les
              documents suivants
            </p>
            <ul class="my-4 list-disc text-gray-600">
              <li>Carte d’identité</li>
              <li>Justificatif de domicile</li>
              <li>
                Si hébergé, carte d’identité de l’hébergeur et
                attestation d’hébergement(date et lieu de naissance
                pour héberger et hébergeur)
              </li>
              <li>Si entre 17ans à 25ans ASSR2</li>
              <li>Si entre 17ans à 25 ans journée d’appel à La Défense</li>
              <li>Photo ANTS (possible dans les photomatons)</li>
            </ul>
          </div>
          <div
            class="grid grid-auto-rows grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-12 pb-8"
          ></div>
        </div>
      </div>
    </div>

    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#F7FAFC"
        fill-opacity="1"
        d="M0,128L288,160L576,64L864,32L1152,96L1440,32L1440,0L1152,0L864,0L576,0L288,0L0,0Z"
      />
    </svg>

 
    <div class="mt-20 ">
      <h1 class="font-bold uppercase text-5xl text-gray-900 px-2 md:px-0 text-center">Contactez-nous</h1>
      <div class="mx-4 md:w-2/3 md:mx-auto shadow-lg rounded-3xl relative">
        <ContactForm />
      </div>
    </div>

    <svg
      class="md:-mt-24 z-10 fill-current text-gray-100"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 1440 320"
    >
      <path
        fill-opacity="1"
        d="M0,96L240,224L480,256L720,192L960,256L1200,288L1440,64L1440,320L1200,320L960,320L720,320L480,320L240,320L0,320Z"
      />
    </svg>
    <div class="footer py-8 bg-gray-100">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 pb-8 w-5/6 mx-auto">
        <div class="justify-center flex flex-col">
          <Logo class="h-48" />
          <h1
            class="font-bold w-full text-center text-gray-900 uppercase text-3xl tracking-wider"
          >AB PERMIS</h1>
        </div>
        <div class="text-center flex flex-col">
          <h2 class="text-lg uppercase font-bold text-primary-500 md:mb-4">HISTORIQUE</h2>
          <div class="text-gray-600 p-4">
            Fondée en 2017,
            <span class="font-bold">AB PERMIS</span>,
            contribue activement à la réussite de ses élèves, une
            pédagogie en adéquation à chaqu'un avec des mises en
            situation qui vous parlerons et vous ferons prendre
            conscience de l'importance de la sécurité routière.
          </div>
          <div class="text-gray-600 p-4">
            Du haut de nos
            <span class="font-bold">
              20 ans
              d’expérience
            </span> cumulée, faites-nous
            confiance pour votre réussite. Satisfait ou satisfait.
          </div>
        </div>
        <div class="text-center flex flex-col">
          <h2 class="text-lg font-bold text-primary-500 md:mb-4">HORAIRES</h2>
          <div class="text-gray-500">Lundi au vendredi</div>
          <div class="text-gray-600">16h à 19h</div>
          <div class="text-gray-500">Samedi</div>
          <div class="text-gray-600">10h à 12h</div>
        </div>
        <div class="text-center flex flex-col">
          <h2 class="text-lg font-bold text-primary-500 md:mb-4">COORDONNÉES</h2>
          <div class="text-gray-500">contact@ab-permis.com</div>
          <div class="text-gray-600">04 77 74 53 73</div>
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
      offersAuto: [
        {
          title: "Évaluation de départ",
          description: "Un premier rendez-vous pour convenir du volume d’heures nécessaire à la suite duquel on signe le contrat de formation",
          price: "40€"
        },
        {
          title: "Formation Permis B, AAC, CS",
          description: "La formation comprend 20 heures de conduite ainsi qu'un support pédagogique",
          price: "880€"
        },
        {
          title: "Rendez-vous pédagogique",
          description: "Obtenez un rendez-vous pédagogique théorique et pratique (destiné aux formation AAC et CS) avec votre accompagnateur",
          price: "80€"
        },
        {
          title: "Heure Supplémentaire",
          description: "Les 20 heures de conduite ne vous suffisent pas ? Formez-vous davantage !",
          price: "45€"
        },
        {
          title: "Examen Supplémentaire Auto",
          description: "Vous avez loupé votre examen ? Ça arrive même aux super héros. Repassez-le tout simplement !",
          price: "45€"
        },
      ],
      offersMoto: [
        {
          title: "Forfait Moto",
          description: "Notre formation moto comprend l'évaluation de départ, 20 heures de pilotage, 1 examen plateau et 1 examen route, ainsi que le code de la route en ligne",
          price: "700€"
        },
        {
          title: "Heure Supplémentaire et initiation",
          description: "Les 20 heures de pilotage ne vous suffisent pas ? Ou vous souhaitez être initié ? Optez pour une heure sur deux roues.",
          price: "40€"
        },
        {
          title: "Examen Supplémentaire Moto",
          description: "Vous avez loupé votre examen ? Ça arrive même aux super héros. Repassez-le tout simplement !",
          price: "50€"
        },
      ],
      offersOther: [
        {
          title: "Frais de dossier",
          description: "Nos frais d'inscriptions, de dossier et de gestion administrative s'élèvent à 40 €",
          price: "40€"
        },
        {
          title: "Forfait Code en salle",
          description: "Participez à cette formation théorique du code de la route valable 12 mois",
          price: "200€"
        },
        {
          title: "Forfait Code en ligne",
          description: "Participer, à votre rythme, à la formation du code de la route en ligne ! Le prix inclus les frais de dossier !",
          price: "70€"
        },
      ]
    };
  },
}
</script>

<style>
.card-image {
  transform: perspective(200px) rotateY(-2deg);
}
</style>
