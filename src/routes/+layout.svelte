<script lang="ts">
  import "iapau-components/css/default-theme.css";
  import "iapau-components/iapau-link";
  import "iapau-components/iapau-button";
  import { page } from "$app/stores";

  const pages = [
    ["Accueil", "/"],
    ["L'association IA Pau", "/iapau/"],
    ["Prochains événements", "/events/"],
    ["Archives", "/archives/"],
    ["Contact", "/contact/"],
  ];

  let current_page: string;
  $: current_page = $page.url.pathname;
  console.log(current_page)

  function page_name(curr: string) {
    let res = "IA PAU";
    console.log(curr)
    pages.forEach((p) => {
      if (p[1] == curr) {
        res = p[0];
      }
    });

    return res;
  }
</script>

<svelte:head>
  <title>{page_name(current_page)}</title>
</svelte:head>

<header
  style="
  position: fixed;
  top: 0;
  z-index: 999;
  background-color: white;
  width: 100%;
  display: flex; flex-direction: row; justify-content: center;
"
>
  <div
    style="display: flex; flex-direction: row; align-items: center; justify-content: space-between;  height: 5em; gap: 3vw;"
  >
    <a style="height: 75%;" href="/"
      ><img alt="" src="/img/iapau_round.png" height="100%" /></a
    >
    <div style="display: flex; align-items: center; gap: 1.5rem">
      {#each pages as page}
        <iapau-link href={page[1]} active={current_page == page[1]}>
          {page[0]}
        </iapau-link>
      {/each}
    </div>
    <iapau-button><a href="/account">Data Challenges</a></iapau-button>
  </div>
</header>

<div style="flex: 1 0; padding-top: 5em">
  <slot />
</div>
<div
  style="background-color: var(--iapau-color-bg-primary); color:white;"
  class="column-center"
>
  <div
    style="height: 100px; width: 100%; background-size: 100% 100px;background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDBweCIgdmlld0JveD0iMCAwIDEyODAgMTQwIiBwcmVzZXJ2ZUFzcGVjdFJhdGlvPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxnIGZpbGw9IiNmZmZmZmYiPjxwYXRoIGQ9Ik05NzguODEgMTIyLjI1TDAgMGgxMjgwbC0yNjIuMSAxMTYuMjZhNzMuMjkgNzMuMjkgMCAwIDEtMzkuMDkgNS45OXoiIGZpbGwtb3BhY2l0eT0iLjUiLz48cGF0aCBkPSJNOTgzLjE5IDk1LjIzTDAgMGgxMjgwbC0yNjYgOTEuNTJhNzIuNTggNzIuNTggMCAwIDEtMzAuODEgMy43MXoiLz48L2c+PC9zdmc+);"
  />
  <div
    style="margin: 5px; text-align: center; font-size: 1.5rem;"
    class="column-center"
  >
    <a href="/contact" class="link">
      <h1>REJOIGNEZ-NOUS</h1>
    </a>
    <div style="height: 5px; width: 90%; background-color: white;" />
    <h1>#IAPAU</h1>
  </div>
</div>

<style global>
  :global(html) {
    height: 100%;
    margin: 0;
  }
  :global(body) {
    height: 100%;
    margin: 0;
    font-family: "Montserrat";
  }

  :global(.column-center) {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  :global(.link) {
    text-decoration: none;
    text-decoration-skip-ink: auto;
    color: inherit;
  }

  .link:hover {
    text-decoration: underline;
  }

  @font-face {
    font-family: "Montserrat";
    src: url("/fonts/Montserrat-Medium.ttf");
  }

  @font-face {
    font-family: "Montserrat";
    src: url("/fonts/Montserrat-Light.ttf");
    font-weight: 300;
  }

  @font-face {
    font-family: "Montserrat";
    src: url("/fonts/Montserrat-Bold.ttf");
    font-weight: bold;
  }

  a {
    text-decoration: none;
    color: var(--ia-pau-bg-default)
  }
</style>
