<script lang="ts">
  export let href: string;
  export let logo: string;
  export let size: string = "35px";
  export let hover = true;
</script>

<a {href} class={hover ? "hover" : ""}>
  <div

    style="height: {size}; width: {size}; mask: url({logo}) no-repeat center; -webkit-mask: url({logo}) no-repeat center;"
  />
</a>

<style>
  a {
    text-decoration: none;
    background-color: var(--iapau-color-bg-default);
    padding: 0.875rem;
    border-radius: 10rem;
    display: block;
    outline: 0;
    height: fit-content;
    transition: 0.3s ease;
  }

  .hover:hover {
    background-color: var(--iapau-color-bg-primary);
  }

  a > div {
    height: 35px;
    width: 35px;
    background-color: var(--iapau-color-bg-primary);
    height: 100%;
  }

  .hover:hover > div {
    background-color: var(--iapau-color-bg-default);
  }
</style>
