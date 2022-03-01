<template>
  <section class="text-gray-600 body-font">
    <div class="flex flex-col justify-center items-center relative z-0">
      <form
        name="contact"
        method="POST"
        action="/merci"
        netlify
        netlify-honeypot="bot-field"
        class="card-glow p-8 rounded-md w-full md:w-2/3"
      >
        <input type="hidden" name="form-name" value="contact" />
        <p class="hidden">
          <label>
            Don’t fill this out if you’re human:
            <input name="bot-field" />
          </label>
        </p>
        <div class="mb-6">
          <label for="name" class="label">Nom</label>
          <input id="name" type="text" name="name" required class="input" />
        </div>
        <div class="mb-6">
          <label for="email" class="label">Email</label>
          <input id="email" type="email" name="email" required class="input placeholder-italic" />
        </div>
        <div class="mb-6">
          <label for="message" class="label">Message</label>

          <textarea id="message" rows="5" name="message" class="input" required></textarea>
        </div>
        <div class="mb-6 relative z-10">
          <button
            type="submit"
            class="w-full px-3 py-4 card-glow uppercase bg-gray-900 text-white rounded-md focus:bg-white focus:text-black focus:outline-gray-900"
          >Envoyer</button>
        </div>
      </form>
    </div>
  </section>
</template>