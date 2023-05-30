<script lang="ts">
  import "iapau-components/iapau-button";
  import "iapau-components/iapau-card";
  import "iapau-components/iapau-input";
  import "iapau-components/iapau-select";

  import HoverIcon from "../../lib/HoverIcon.svelte";
  import PageCard from "../../lib/PageCard.svelte";
  import linkedin from "remixicon/icons/Logos/linkedin-fill.svg";
  import mail from "remixicon/icons/Business/mail-fill.svg";
  import facebook from "remixicon/icons/Logos/facebook-fill.svg";
  import map from "remixicon/icons/Map/map-pin-2-fill.svg";
  import share from "remixicon/icons/System/share-fill.svg";

  const options = ["Je veux rejoindre l'asso"];
</script>

<div
  style="height: 75vh; 
  background-position: center top;
  background-image: radial-gradient(circle at top right,rgba(255,255,255,0) 20%,#0e8769 100%),url(/img/our_events.jpg) !important;"
  class="column-center"
>
  <div
    style="flex: 1; align-items: start !important; width: 55%; color:white;"
    class="column-center"
  >
    <h3 style="opacity: 0.8;">Toujours à votre écoute</h3>
    <h1 style="font-size: 3rem; margin: 0px; font-weight: bold;">
      Contactez-nous !
    </h1>
    <div
      style="display: flex; justify-content: space-evenly; gap: 3rem; margin-top: 2rem;"
    >
      <HoverIcon
        href="https://fr.linkedin.com/company/ia-pau"
        logo={linkedin}
      />
      <HoverIcon href="https://iapau.org/contact/" logo={mail} />
      <HoverIcon
        href="https://www.facebook.com/IA-Pau-1494793403982576/?__xts__[0]=68.ARDOq4I4L0WvUT0kqdblc1P_L2uITLG-XGleZvuM_wIs6FuGYU3rcmhGZlsgo6dvZORji6E_WPOfEvA8YvvTw8Cy6e8yAbqbA2PbyW380s-J4LRXrurT7GaSpWbl9ByP0-XauAjmN_Y3XQDxOwSuE3pc2DNTJDtAAsozxUl1-NjHn1Mwz25dMA"
        logo={facebook}
      />
    </div>
  </div>
  <div
    style="height: 50px; width: 100%; transform: scale(-1,1); background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSI1MHB4IiB2aWV3Qm94PSIwIDAgMTI4MCAxNDAiIHByZXNlcnZlQXNwZWN0UmF0aW89Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0iI2VkZWZmYSI+PHBhdGggZD0iTTEyODAgMGwtMjYyLjEgMTE2LjI2YTczLjI5IDczLjI5IDAgMCAxLTM5LjA5IDZMMCAwdjE0MGgxMjgweiIvPjwvZz48L3N2Zz4=);
background-size: 100% 50px;"
  />
</div>

<div class="column-center">
  <h1
    style="font-size: 3rem; margin: 0px; font-weight: bold; margin-bottom: 3rem; margin-top: 6rem;"
  >
    Envoyez un message
  </h1>
  <div
    style="display: flex; width: auto; padding: 2rem; box-shadow: 0px 2px 70px 0px rgba(110,130,208,0.18); border-radius: 15px;"
    class="column-center"
  >
    <div style="display: flex; gap: 1rem;">
      <iapau-input placeholder="Nom" />
      <iapau-input placeholder="Email" />
    </div>
    <iapau-select label="C'est à quel sujet ?" {options} />
  </div>
  <div
    style="width: 60%; display: flex; justify-content: space-evenly; margin: 10rem;"
  >
    <PageCard
      title="Retrouvez-nous"
      hoverUpAnimation={false}
      height="260px"
      style="min-height: 0px !important;"
    >
      <div slot="header" class="column-center" style="height: 100%">
        <HoverIcon hover={false} href="." logo={map} size="65px" />
      </div>
      <p slot="content">
        <iapau-link active>2 avenue Président Pierre Angot</iapau-link>
        <br />
        <iapau-link active>64 000 Pau</iapau-link>
      </p>
    </PageCard>
    <PageCard
      title="Contactez-nous"
      hoverUpAnimation={false}
      height="260px"
      style="min-height: 0px !important;"
    >
      <div slot="header" class="column-center" style="height: 100%">
        <HoverIcon hover={false} href="." logo={mail} size="65px" />
      </div>
      <p slot="content">
        Par formulaire ou <br />
        contact@iapau.org
      </p>
    </PageCard>
    <PageCard
      title="Suivez-nous"
      hoverUpAnimation={false}
      height="260px"
      style="min-height: 0px !important;"
    >
      <div slot="header" class="column-center" style="height: 100%">
        <HoverIcon hover={false} href="." logo={share} size="65px" />
      </div>
      <p slot="content">
        <iapau-link active>LinkedIn</iapau-link>
        <br>
        <iapau-link active>Twitter</iapau-link>
      </p>
    </PageCard>
  </div>
</div>

<style>
  iapau-input {
    width: 75%;
    min-width: 350px;
    margin-top: 0.875rem;
    display: flex;
  }

  iapau-select {
    width: 100%;
    min-width: 350px;
    margin-top: 0.875rem;
    display: flex;
  }

  p {
    text-align: center;
  }
</style>
