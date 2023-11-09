<html lang>

<div class="mainIndexContainer">

    <div class="mainIndexHeader">
        
        <div class="headerImages">
            
            <img class="containImg indexLogoImg" src="../img/indexlogo.png" alt="title icon">

            <div class ="mainIndexButtonsContainer">
            
                <a href="suits"><button class="indexNavigationButtons">Mobile Suits</button></a>
                <a href="titles"><button class="indexNavigationButtons">Titles</button></a>
                <a href="shows"><button class="indexNavigationButtons">Shows</button></a>
                <a href="about"><button class="indexNavigationButtons">About</button></a>
                <a href="/"><button class="homeButton"></button></a>
        
            </div>
        
        </div>

    </div>

    <div class="suitsContainer">

        <div class="suitsContainerDivs">

            <div id="characterContainer">

                Content

                <div id="charImage">

                    <h1 id="charName">Gundam Kyrios</h1>
                    <img src="../img/Kyrios.png" alt="char1">
                    
                </div>

                <button class="buttonChar" onclick="ChangeCharacter('Kyrios')">Kyrios</button>
                <button class="buttonChar" onclick="ChangeCharacter('Freedom')">Freedom</button>



            </div>

        </div>

        <div class="suitsContainerDivs">

        </div>
        
    </div>


</div>

<script>

    function ChangeCharacter(character)
    {
    switch(character)
    {
        case "Kyrios":
            document.getElementById("charImage").src = "../img/Kyrios.png";
            document.getElementById("charName").innerHTML = "Kyrios";
            break;
        case "Freedom":
            document.getElementById("charImage").src = "../img/Freedom.png";
            document.getElementById("charName").innerHTML = "Freedom";
            break;
    
    }
    }
        </script>
    

</html>