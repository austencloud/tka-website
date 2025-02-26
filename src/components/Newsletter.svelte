<script>
  let email = "";

  function handleSubmit() {
    alert(`Subscribed: ${email}`);
    email = "";
  }
</script>

<form on:submit|preventDefault={handleSubmit} class="newsletter-form">
  <h3>Stay in the loop</h3>
  <p>Sign up with your email to receive updates.</p>
  <input type="email" bind:value={email} placeholder="Enter your email" required />
  <button type="submit">Subscribe</button>
</form>

<style>
  .newsletter-form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  input {
    padding: 10px;
    width: 100%;
  }
  button {
    background: #A81CED;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
  }
</style>