<script>

    import { onMount } from "svelte";

    let allData = [];     //Variable to store fetched data 
    const BASE_URL = "https://api.unsplash.com/search/photos";
    const API_KEY = "wjv4ZtTX-i5cyFTaY_20ByyPc3cnvHLcOOb95dkINx8";
    const query = "gundam";

    onMount(async () => {     //Execute when component is mounted
      try {
        const response = await fetch(
          `${BASE_URL}?query=${query}&client_id=${API_KEY}` //Fetch data from from Unsplash
        );
        if (response.ok) {
          const data = await response.json(); //If data is successfully fetched, display the fetched data results
          allData = data.results;
        } else {
          console.error("Error fetching data:", response.statusText); //If unsuccessful, display error message
        }
      } catch (error) {
        console.error("Error fetching data:", error);
      }
    });

    function ChangeCharacter(character) {     //Function that is supposed to change source images and names of Gundam based on which button is clicked
      switch (character) {
        case "Freedom":
          document.getElementById("charImage").src = "/img/Freedom.png"; //Ex. If Freedom button is clicked, changed image source to Freedom Gundam image location.png
          document.getElementById("charName").innerHTML = "Freedom";
          break;

        case "Kyrios":
          document.getElementById("charImage").src = "/img/Kyrios.png";
          document.getElementById("charName").innerHTML = "Kyrios";
          break;
      }
    }
  </script>

  <div class="mainIndexContainer">
    <div class="mainIndexHeader">
      <div class="headerImages">
        <img
          class="containImg indexLogoImg"
          src="../img/indexlogo.png"
          alt="title icon"
        />

        <div class="mainIndexButtonsContainer">
          <a href="suits"
            ><button class="indexNavigationButtons">Mobile Suits</button></a
          >
          <a href="titles"
            ><button class="indexNavigationButtons">Titles</button></a
          >
          <a href="shows"
            ><button class="indexNavigationButtons">Shows</button></a
          >
          <a href="about"
            ><button class="indexNavigationButtons">About</button></a
          >
          <a href="/"><button class="homeButton" /></a>
        </div>
      </div>
    </div>

    <div class="suitsContainer">
      <div class="suitsContainerDivs">
        <div id="characterContainer">
          Content

          <div id="charImage">
            <h1 id="charName">Freedom Gundam</h1>
            <img src="../img/Freedom.png" alt="Freedom Gundam">
          </div>

          <button class="buttonChar" onclick="ChangeCharacter('Kyrios')"
            >Kyrios</button
          >
          <button class="buttonChar" onclick="ChangeCharacter('Freedom')"
            >Freedom</button
          >
          <button class="buttonChar" onclick="ChangeCharacter('Freedom')"
            >Justice</button
          >
          <button class="buttonChar" onclick="ChangeCharacter('Freedom')"
            >Barbatos</button
          >
        </div>
      </div>

      <div class="suitsContainerDivs">
        {#each allData as image}
          <img src={image.urls.small} alt="Gundam" width="300" height="270"/>
        {/each}
      </div>
    </div>
  </div>

  
 