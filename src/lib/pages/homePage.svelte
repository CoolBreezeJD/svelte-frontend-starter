<script>
    import MainNav from "../navigation/mainNav.svelte";
    import MainFooter from "../navigation/mainFooter.svelte";
    import {push, pop, replace} from "svelte-spa-router";

    const openComponentLibrary = () => {
        push("/component-library");
    }
</script>

<MainNav></MainNav>
<main class="mt-5 mb-16 pl-5 pr-5">
    <div class="hero max-h-screen h-96 bg-base-200">
        <div class="text-center hero-content">
          <div class="max-w-md">
            <h1 class="text-5xl font-bold">Welcome</h1>
            <p class="py-6">This is a "blank" home page to get you started. Go nuts!</p>
            <button class="btn btn-primary" on:click={openComponentLibrary}>See Component Library</button>
          </div>
        </div>
      </div>
</main>

<MainFooter/>