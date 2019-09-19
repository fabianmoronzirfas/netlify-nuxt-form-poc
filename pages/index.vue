<template>
  <div class="container">
    <div>
      <form
        name="contactus"
        action="/"
        method="post"
        netlify
        netlify-honeypot="bot-field"
      >
        <!-- Hidden input to check for bots -->
        <input type="hidden" name="form-name" value="contactus" />
        <div>
          <label for="name">Name:</label>
          <input type="text" name="name" required />
        </div>
        <div>
          <label for="email">Email:</label>
          <input type="email" name="email" required />
        </div>
        <div>
          <label for="message">Message:</label>
          <textarea name="message" required></textarea>
        </div>
        <button type="submit" value="Send message">Send</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Form'
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
