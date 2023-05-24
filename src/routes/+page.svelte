<script lang="ts">
  import "iapau-components/iapau-button";
  import "iapau-components/iapau-card";
  import HoverIcon from "../lib/HoverIcon.svelte";
  import PageCard from "../lib/PageCard.svelte";
  import linkedin from "remixicon/icons/Logos/linkedin-fill.svg";
  import mail from "remixicon/icons/Business/mail-fill.svg";
  import facebook from "remixicon/icons/Logos/facebook-fill.svg";
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
<div class="column-center">
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
    <br />
    scientifiques, technologiques, éthiques, et démocratiques.<br />
  </p>
  <div
    style="display:flex; width: 50%; justify-content: space-evenly; height: 45px; margin-top: 1rem; margin-bottom: 5rem;"
  >
    <HoverIcon href="https://fr.linkedin.com/company/ia-pau" logo={linkedin} />
    <HoverIcon href="https://iapau.org/contact/" logo={mail} />
    <HoverIcon
      href="https://www.facebook.com/IA-Pau-1494793403982576/?__xts__[0]=68.ARDOq4I4L0WvUT0kqdblc1P_L2uITLG-XGleZvuM_wIs6FuGYU3rcmhGZlsgo6dvZORji6E_WPOfEvA8YvvTw8Cy6e8yAbqbA2PbyW380s-J4LRXrurT7GaSpWbl9ByP0-XauAjmN_Y3XQDxOwSuE3pc2DNTJDtAAsozxUl1-NjHn1Mwz25dMA"
      logo={facebook}
    />
  </div>
</div>
<div
  style="background-color: var(--iapau-color-bg-primary); height: fit-content; min-height:400px;"
  class="column-center"
>
  <div
    style=" height: 100px; width: 100%;background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDBweCIgdmlld0JveD0iMCAwIDEyODAgMTQwIiBwcmVzZXJ2ZUFzcGVjdFJhdGlvPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxnIGZpbGw9IiNmZmZmZmYiPjxwYXRoIGQ9Ik05NzguODEgMTIyLjI1TDAgMGgxMjgwbC0yNjIuMSAxMTYuMjZhNzMuMjkgNzMuMjkgMCAwIDEtMzkuMDkgNS45OXoiIGZpbGwtb3BhY2l0eT0iLjUiLz48cGF0aCBkPSJNOTgzLjE5IDk1LjIzTDAgMGgxMjgwbC0yNjYgOTEuNTJhNzIuNTggNzIuNTggMCAwIDEtMzAuODEgMy43MXoiLz48L2c+PC9zdmc+);
background-size: 100% 100px;"
  />
  <div style="flex: 1; width: 40%; height: auto;" class="column-center">
    <iframe
      style="border: none; aspect-ratio: 16/9; width: 100%;"
      title="Rewind IAPAU#3"
      src="https://www.youtube.com/embed/CxMZnR713Xs?feature=oembed"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      name="fitvid0"
    />
  </div>
  <div
    style="background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSI0NXB4IiB2aWV3Qm94PSIwIDAgMTI4MCAxNDAiIHByZXNlcnZlQXNwZWN0UmF0aW89Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0iI2ZmZmZmZiI+PHBhdGggZD0iTTEwOTQuNDQgMTE5TDE3Mi43IDY4LjcyYTc0LjU0IDc0LjU0IDAgMCAxLTI1LjE5LTUuOTVMMCAwdjE0MGgxMjgwVjBsLTEzMy44NSAxMDJjLTE1Ljg0IDEyLjA5LTMzLjcgMTcuOTUtNTEuNzEgMTd6IiBmaWxsLW9wYWNpdHk9Ii41Ii8+PHBhdGggZD0iTTEwOTMuNDggMTMxLjg1TDE3MyA5NGE3Ni44NSA3Ni44NSAwIDAgMS0zNi43OS0xMS40NkwwIDB2MTQwaDEyODBWMGwtMTMxLjgxIDExMS42OGMtMTYuNDcgMTMuOTYtMzUuNDcgMjAuOTYtNTQuNzEgMjAuMTd6Ii8+PC9nPjwvc3ZnPg==);
  background-size: 100% 45px;
  height: 45px; width:100%;"
  />
</div>
<div
  style="display:flex; align-items: center; margin-top: 5vh; margin: 100px 40px; justify-content: center; gap: 40px;"
>
  <div>
    <h1 style="font-size: 2rem">Pourquoi IA Pau ?</h1>
    <p style="font-weight: 300; font-size: 1.3rem;">
      L’intelligence artificielle, de plus en plus présente dans<br /> notre
      quotidien et dans les médias, suscite de nombreuses <br /> interrogations.
      Alors qu’elle est parfois présentée comme <br /> une simple évolution de
      l’informatique, seulement capable <br /> de reproduire des comportements
      observés dans une <br />grande quantité de données, les progrès réalisés
      ces cinq<br /> dernières années par l’IA questionnent sur les ingrédients
      et <br /> les limites des technologies de l’intelligence artificielle.
    </p>
    <p style="font-weight: 300; font-size: 1.3rem;">
      L’ association IA PAU a pour ambition de démystifier <br />l’intelligence
      artificielle en la rendant accessible au plus<br /> grand nombre en
      proposant des événements <br /> d’acculturation, d’information et de
      partage. Elle favorise et <br /> accompagne également des projets
      collaboratifs entre <br /> entreprises, associations, collectivités et
      étudiants pour <br /> faciliter les échanges dans le domaine de
      l’Intelligence <br /> Artificielle et pour instaurer une dynamique
      collective <br /> pérenne dans le territoire
    </p>
  </div>
  <div>
    <img style="width: 30vw;" src="/img/why_ia_pau.jpg" />
  </div>
</div>
<div
  style="background-color: var(--iapau-color-bg-primary); height: fit-content; min-height:400px; color: white;"
  class="column-center"
>
  <div
    style="background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSI0NXB4IiB2aWV3Qm94PSIwIDAgMTI4MCAxNDAiIHByZXNlcnZlQXNwZWN0UmF0aW89Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0iI2ZmZmZmZiI+PHBhdGggZD0iTTEwOTMuNDggMTMxLjg1TDE3MyA5NGE3Ni44NSA3Ni44NSAwIDAgMS0zNi43OS0xMS40NkwwIDBoMTI4MGwtMTMxLjgxIDExMS42OGMtMTYuNDcgMTMuOTYtMzUuNDcgMjAuOTYtNTQuNzEgMjAuMTd6IiBmaWxsLW9wYWNpdHk9Ii41Ii8+PHBhdGggZD0iTTEwOTQuNDQgMTE5TDE3Mi43IDY4LjcyYTc0LjU0IDc0LjU0IDAgMCAxLTI1LjE5LTUuOTVMMCAwaDEyODBsLTEzMy44NSAxMDJjLTE1Ljg0IDEyLjA5LTMzLjcgMTcuOTUtNTEuNzEgMTd6Ii8+PC9nPjwvc3ZnPg==);
  background-size: 100% 45px;
  height: 45px; width:100%;"
  />
  <h1 style="margin-top: 40px  ">Découvrez notre écosystème</h1>


  <div
    style="display:flex; align-items: center; margin: 5vh 0; justify-content: space-evenly; width: auto; padding: 0px 10vw; gap: 20px;"
  >
    <PageCard title="Nos évènements">
      <img
        slot="header"
        style="height: 100%; width: 100%;"
        src="/img/our_events.jpg"
      />
      <p slot="content">
        Prochain festival, prochain Meetup <br /> ou prochain Data Challenge ?
        <br />
        Tous les évènements à venir<br /> d’IA Pau sont par ici, et <br /> n’attendent
        plus que vous !
      </p>
    </PageCard>
    <PageCard title="Nos évènements">
      <img
        slot="header"
        style="height: 100%; width: 100%;"
        src="/img/our_archives.jpeg"
      />
      <p slot="content">
        Prochain festival, prochain Meetup <br /> ou prochain Data Challenge ?
        <br />
        Tous les évènements à venir<br /> d’IA Pau sont par ici, et <br /> n’attendent
        plus que vous !
      </p>
    </PageCard>
    <PageCard title="Nos évènements">
      <img
        slot="header"
        style="height: 100%; width: 100%;"
        src="/img/discover_us.jpg"
      />
      <p slot="content">
        Prochain festival, prochain Meetup <br /> ou prochain Data Challenge ?
        <br />
        Tous les évènements à venir<br /> d’IA Pau sont par ici, et <br /> n’attendent
        plus que vous !
      </p>
    </PageCard>
  </div>
  <div
    style="background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAwJSIgaGVpZ2h0PSI0NXB4IiB2aWV3Qm94PSIwIDAgMTI4MCAxNDAiIHByZXNlcnZlQXNwZWN0UmF0aW89Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0iI2ZmZmZmZiI+PHBhdGggZD0iTTEwOTQuNDQgMTE5TDE3Mi43IDY4LjcyYTc0LjU0IDc0LjU0IDAgMCAxLTI1LjE5LTUuOTVMMCAwdjE0MGgxMjgwVjBsLTEzMy44NSAxMDJjLTE1Ljg0IDEyLjA5LTMzLjcgMTcuOTUtNTEuNzEgMTd6IiBmaWxsLW9wYWNpdHk9Ii41Ii8+PHBhdGggZD0iTTEwOTMuNDggMTMxLjg1TDE3MyA5NGE3Ni44NSA3Ni44NSAwIDAgMS0zNi43OS0xMS40NkwwIDB2MTQwaDEyODBWMGwtMTMxLjgxIDExMS42OGMtMTYuNDcgMTMuOTYtMzUuNDcgMjAuOTYtNTQuNzEgMjAuMTd6Ii8+PC9nPjwvc3ZnPg==);
  background-size: 100% 45px;
  height: 45px; width:100%;"
  />
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
