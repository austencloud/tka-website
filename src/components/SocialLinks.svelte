<script>
  let socialLinks = [
    { name: "YouTube", href: "http://youtube.com/thekineticalphabet", icon: "youtube" },
    { name: "Instagram", href: "http://instagram.com/thekineticalphabet", icon: "instagram" },
    { name: "Facebook", href: "http://facebook.com/thekineticalphabet", icon: "facebook" },
    { name: "TikTok", href: "http://tiktok.com/thekineticalphabet", icon: "tiktok" }
  ];
</script>

<div class="social-links">
  {#each socialLinks as link}
    <a href={link.href} target="_blank" aria-label={link.name}>
      <i class="icon-{link.icon}"></i>
    </a>
  {/each}
</div>

<style>
  .social-links {
    display: flex;
    gap: 10px;
  }
  a {
    color: white;
    font-size: 1.5rem;
  }
</style>
