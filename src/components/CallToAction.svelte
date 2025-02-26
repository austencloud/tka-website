<script>
  export let text;
  export let link;
</script>

<a href={link} target="_blank" class="cta-button">{text}</a>

<style>
  .cta-button {
    display: inline-block;
    padding: 10px 20px;
    background: #A81CED;
    color: white;
    border-radius: 5px;
    text-decoration: none;
    text-align: center;
  }
  .cta-button:hover {
    background: #8c0bcf;
  }
</style>
