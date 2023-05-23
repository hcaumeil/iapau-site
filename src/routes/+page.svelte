<script lang="ts">
  import "iapau-components/iapau-button";
  import HoverIcon from "../lib/HoverIcon.svelte";
  import linkedin from "remixicon/icons/Logos/linkedin-fill.svg"
  import mail from "remixicon/icons/Business/mail-fill.svg"
  import facebook from "remixicon/icons/Logos/facebook-fill.svg"
</script>

<div
  style="background-image: url('/img/pyrenees.jpg');  color:white; height: calc(100vh - 100px);"
  class="parallax"
>
  <div
    style="height: 100%; background-color: rgba(0,0,0,0.3); text-align: center;"
    class="column-center"
  >
    <div style="flex:1 0" class="column-center">
      <h1 style="font-size: 5rem; margin: 0;">IA PAU</h1>
      <p style="font-size: 2rem; margin: 0.875rem; font-weight: 300;">
        L'intelligence artificielle vue des Pyrénées
      </p>
      <iapau-button size="lg" style="margin: 0.875rem;">
        <a href="https://www.meetup.com/fr-FR/meetup-machine-learning-pau/"
          >Prochain évènement</a
        >
      </iapau-button>
    </div>
    <div
      style="width:100%; background-size: 100% 100px; height: 100px; background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDBweCIgdmlld0JveD0iMCAwIDEyODAgMTQwIiBwcmVzZXJ2ZUFzcGVjdFJhdGlvPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxnIGZpbGw9IiNGRkZGRkYiPjxwYXRoIGQ9Ik0xMjgwIDBsLTI2NiA5MS41MmE3Mi41OSA3Mi41OSAwIDAgMS0zMC43NiAzLjcxTDAgMHYxNDBoMTI4MHoiIGZpbGwtb3BhY2l0eT0iLjUiLz48cGF0aCBkPSJNMTI4MCAwbC0yNjIuMSAxMTYuMjZhNzMuMjkgNzMuMjkgMCAwIDEtMzkuMDkgNkwwIDB2MTQwaDEyODB6Ii8+PC9nPjwvc3ZnPg==);"
    />
  </div>
</div>
<div style="height: 600px" class="column-center">
  <h1 style="color: var(--iapau-color-bg-primary); font-size: 3rem">IA PAU</h1>
  <p style="font-weight: 300; font-size: 1.3rem; text-align:center">
    L’association IA PAU rassemble dans la bonne humeur <br />
    chercheurs, enseignants, étudiants, entrepreneur et particuliers<br />
    autour de la thématique du traitement des données <br />
    et propose de rapprocher la sphère économique, le monde académique <br />
    et le grand public en organisant des événements et des projets collaboratifs.
    <br />
    <br />
    Son objectif est de vulgariser et partager les connaissances<br />
    autour de ce progrès majeur du XXIème siècle qui suscite de nombreuses interrogations 
    <br/>
    scientifiques, technologiques, éthiques, et démocratiques.<br />
  </p>
  <div style="display:flex; width: 50%; justify-content: space-evenly; height: min(45px, 10vh); margin-top: 1rem">
    <HoverIcon href="https://fr.linkedin.com/company/ia-pau" logo={linkedin} />
    <HoverIcon href="https://iapau.org/contact/" logo={mail} />
    <HoverIcon href="https://www.facebook.com/IA-Pau-1494793403982576/?__xts__[0]=68.ARDOq4I4L0WvUT0kqdblc1P_L2uITLG-XGleZvuM_wIs6FuGYU3rcmhGZlsgo6dvZORji6E_WPOfEvA8YvvTw8Cy6e8yAbqbA2PbyW380s-J4LRXrurT7GaSpWbl9ByP0-XauAjmN_Y3XQDxOwSuE3pc2DNTJDtAAsozxUl1-NjHn1Mwz25dMA" logo={facebook} />
  </div>
</div>

<style>
  .parallax {
    min-height: 6rem;

    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }

  @media only screen and (max-device-width: 1366px) {
    .parallax {
      background-attachment: scroll;
    }
  }

  a {
    color: inherit;
    text-decoration: inherit; /* no underline */
  }
</style>
