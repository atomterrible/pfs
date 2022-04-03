<template>
  <section class="w-full bg-primary-700 p-6 lg:p-14">
    <div class="box">
      <h1>Contact</h1>
      <p class="text-xl">
        If you'd like to learn more about my services and pricing, please visit the
        <a href="/services">Services</a> page. If you'd like to book, please call or text
        <a href="tel:19403674447">940-367-4447</a>. For all other questions, please use the form below.
      </p>
      <br />
      <form name="Contact" method="POST" data-netlify="true" netlify>
        <label class="hidden"> Don’t fill this out if you’re human: <input name="bot-field" /> </label>
        <label for="name">Full Name</label>
        <input class="p-2" type="text" id="name" name="name" placeholder="Your name.." />

        <label for="email">Email</label>
        <input class="p-2" type="text" id="email" name="email" placeholder="Your email.." />

        <label for="subject">Message</label>
        <textarea
          class="p-2"
          id="subject"
          name="subject"
          placeholder="How can I help?"
          style="height: 200px"
        ></textarea>

        <input class="btn" type="submit" value="Send" />
      </form>
    </div>
  </section>
</template>

<style lang="postcss" scoped>
</style>

<script>
export default {}
</script>