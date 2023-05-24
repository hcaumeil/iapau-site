<script lang="ts">
  export let title : string = "";
  export let href : string = ".";
</script>

<style>
a {
  text-decoration: none;
  color: black;
}
</style>

<iapau-card
  style="max-height: 600px; min-height: 300px; max-height: 600px; width: 18vw; overflow: hidden;"
  hoverUpAnimation
>
  <a class="column-center" style="height: 100%; justify-content: start !important;" href={href} target="_blank">
    <div style="height: 50%; width: 100%; position: relative;" >
      <slot name ="header"/>
    </div>
    <div style="height: 50%; text-align: center;" class="column-center">
      <h3>{title}</h3>
      <slot name="content"/>
    </div>
  </a>
</iapau-card>
