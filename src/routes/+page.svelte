<script lang="ts">
  import "iapau-components/iapau-button";
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
<div style="height: 80vh" class="column-center">
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
