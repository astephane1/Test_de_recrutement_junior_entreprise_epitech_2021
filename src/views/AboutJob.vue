<template>
<div id="app">
<div id="card_info">
<img src="../assets/sodson.jpeg" alt="you">
<div id="card_if">
  <b-card-group deck>
    <b-card
      header="SODSON CORP"
      header-tag="header"
      footer="Cotonou, Bénin"
      footer-tag="footer"
    >
      <b-card-text>
      <h5>Présentation de la structure : </h5><br/>
       <p>● Entreprise d'ingénierie logicielle à part entière, nos différents projets nous ont permis d'éteindre notre offre de service sur les segments d'infrastructures, de systèmes biométriques, de documents sécurisés (visa, passeport) et plus globalement sur toutes branches de l'industrie du logiciel.</p>
        <h5>Missions du stagiaires :</h5><br/>
      ● Aider à rédiger un code bien conçu, testable et efficace en utilisant les meilleures pratiques de développement logiciel.</b-card-text>
    </b-card>
  </b-card-group><br/>
  <b-button href="#" variant="success">POSTULEZ</b-button>
  </div>
</div>
</div>
</template>

<style>

#card_if {
    width:40%;
    height:100%;
    display:relative;
    position:relative;
    left:30%;
    top:1%;

}

#card_if b-button {
     position:relative;
     top:-100%;
}

.row {
color: green;
}

#card_info img {
    position:relative;
    height:18%;
    width:18%;
    left:10%;
    top:1%;

}

#card_info {
    position:relative;
    top: 90px;
    display: flex;
}

</style>

<script>
</script>