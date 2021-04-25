<template>
<div id="app">
<div id="card_info">
<img src="../assets/Epitech.png" alt="you">
<div id="card_if">
  <b-card-group deck>
    <b-card
      header="Epitech bénin"
      header-tag="header"
      footer="Lieu : Cotonou, Bénin"
      footer-tag="footer"
    >
      <b-card-text>
      <h5>Présentation de la structure : </h5><br/>
        <p>● Epitech, l’école référence de l'expertise informatique,
forme depuis 20 ans les experts qui dessineront
le monde de demain.</p><br/>
        <h5>Missions du stagiaires :</h5><br/>
      ● Être AER (Assistants Epitech en Région) : Véritables piliers de la pédagogie par projets d'Epitech, les AER sont des étudiants de promotions supérieures qui partagent et transmettent leurs compétences aux autres étudiants.</b-card-text>
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

export default {
	data ()
         {
           return {
             InfoEntreprise: [
                { label: 'développeur web junior', entreprise: 'Sodson Corp', img_path: "../assets/Epitech.png", url:"/aboutjob" },
                { label: 'Assistant pédagogique', entreprise: 'Epitech bénin', img_path: "../assets/Epitech.png", url:"/aboutjob1" },
                { label: 'Technicien réseau junior', entreprise: 'Bénin Télécom', img_path: "../assets/Epitech.png", url:"/aboutjob2" }
            ]
           }
           }

    }

</script>