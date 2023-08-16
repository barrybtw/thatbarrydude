<script  lang="ts">
  import Sun from "./sun.svelte"
  import Moon from "./moon.svelte"

  function changeTheme() {
    document.documentElement.classList.toggle("dark")
    localStorage.setItem("theme", document.documentElement.classList.contains("dark") ? "dark" : "light")
  }
</script>
<nav class="flex w-full mb-8 md:mb-12 h-12 lowercase items-center">
  <div class="flex w-full justify-between items-center">
    <div class="flex items-center">
      <a href="/" class="md:text-3xl text-xl lg:text-4xl font-semibold">thatbarrydude</a>
    </div>
    <div class="flex items-center gap-4 md:gap-8">
      <button on:click={changeTheme}>
        <Sun class="dark:inline-block hidden md:h-5 h-4 w-4 md:w-5" />
        <Moon class="dark:hidden md:h-5 h-4 w-4 md:w-5 inline-block" />
      </button>
    </div>
  </div>
</nav>