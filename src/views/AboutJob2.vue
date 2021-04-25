<template>
<div>
<div id="card_info">
<img src="../assets/Benin_Telecoms.png" alt="imgentreprise">
<div id="card_if">
  <b-card-group deck>
    <b-card
      header="Bénin Télécom"
      header-tag="header"
      footer="Lieu : Cotonou, Bénin"
      footer-tag="footer"
    >
  <b-card-text>
      <h5>Présentation de la structure : </h5>
       <p>● L'Office des Postes et Télécommunications de la République du Bénin (OPT) </p>
        <h5>Missions du stagiaires :</h5><br/>
      ● Veiller au bon fonctionnement de serveurs, des postes de travail, du réseau informatique dans  sa  globalité  et  des  communications  (voix  et  données).</b-card-text>
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