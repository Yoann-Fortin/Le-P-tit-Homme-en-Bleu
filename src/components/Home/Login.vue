<template>
  <form action="" method="post">
    <legend>Inscription</legend>
    <label id="pseudo-label" for="">Pseudo</label>
    <input id="pseudo-input" type="text">
    <label id="email-label" for="">Email</label>
    <input id="email-input" type="text">
    <label id="password-label" for="">Mot de Passe</label>
    <input id="password-input" type="text">
    <label id="confirm-label" for="">Confirmez le Mot de Passe</label>
    <input id="confirm-input" type="text">
    <button type="submit">S'inscrire</button>
    <a href="">Déjà inscrit? Cliquez ici</a>
  </form>
</template>

<script>
export default {
  name: 'Login'
}
</script>

<style scoped>
  form {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(8, 1fr);
    margin: 2rem;
    margin-top: 0;
    background-color: #060668;
    border-radius: 50%;
    padding: 2rem;
    min-width: 25rem;
    max-width: 25rem;
    min-height: 25rem;
    max-height: 25rem;
  }
    
  legend {
    color: #d9e0f3;
    font-family: 'Playfair Display', serif;
    font-weight: bold;
    font-size: 3rem;
    margin: 1rem;
    grid-column-start: 1;
    grid-column-end: end;
    grid-row-start: 1;
    grid-row-end: 3;
    justify-self: center;
    align-self: center;
  }

  label {
    color: #d9e0f3;
    font-weight: bold;
    font-size: 1rem;
    margin: 0 0.5rem;
    height: 2rem;
  }

  input {
    height: 1.5rem;
    margin: 0 0.5rem;
  }

  #pseudo-label {
    grid-column: 1;
    grid-row: 3;
  }

  #pseudo-input {
    grid-column-start: 1;
    grid-column-end: span 2;
    grid-row: 4;
  }

  #email-label {
    grid-column: 3;
    grid-row: 3;
  }

  #email-input {
    grid-column-start: 3;
    grid-column-end: span 2;
    grid-row: 4;
  }

  #password-label {
    grid-column: 1;
    grid-row: 5;
  }

  #password-input {
    grid-column-start: 1;
    grid-column-end: span 2;
    grid-row: 6;
  }

  #confirm-label {
    grid-column-start: 3;
    grid-column-end: span 2;
    grid-row: 5;
  }

  #confirm-input {
    grid-column-start: 3;
    grid-column-end: span 2;
    grid-row: 6;
  }

  button {
    grid-column-start: 2;
    grid-column-end: span 2;
    grid-row: 7;
    background-color: blue;
    color: #d9e0f3;
    font-weight: bold;
    font-size: 1.2rem;
    border-radius: 50%;
    border: solid 1px blue;
  }

  a {
    grid-row: 8;
    grid-column-start: 1;
    grid-column-end: end;
    justify-self: center;
    align-self: center;
    color: #d9e0f3;
  }
</style>