<script>
    const nav = [
    {
      title: 'Портфолио',
      href: '/first',
	  isShow: true,

    },
    ]
</script>


<style>
	.container {
	  max-width: 1400px;
	  margin: 50px auto;
	}

</style>

<nav>
	<div class="nav-container">
	  <a href="/" class="nav-logo" title="На главную страницу">На главную страницу</a>
	  <div class="nav-links">
		{#each nav as link}
			{#if link.isShow}
			<a href={link.href} class="link">{link.title}</a>
			{/if}
		{/each}
	  </div>
	</div>
  </nav>

  <div class="container">
	<!-- Pages will be injected below -->
	<slot></slot>
  </div> 
  
  
  