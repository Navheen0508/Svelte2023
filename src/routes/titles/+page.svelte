<html lang="test">

<div class="mainIndexContainer">

    <div class="mainIndexHeader">
        
        <div class="headerImages">
            
            <img class="containImg indexLogoImg" src="../img/indexlogo.png" alt="title icon">
        
        </div>

        <div class ="mainIndexButtonsContainer">
            
            <a href="suits"><button class="indexNavigationButtons">Mobile Suits</button></a>
            <a href="titles"><button class="indexNavigationButtons">Titles</button></a>
            <a href="shows"><button class="indexNavigationButtons">Shows</button></a>
            <a href="about"><button class="indexNavigationButtons">About</button></a>
            <a href="/"><button class="homeButton"></button></a>

        </div>

    </div>

    <div class="titlesContainer">

        <div>
            
            <h2>Gundam Versus</h2>
            <iframe width="550" height="400"src="https://www.youtube.com/embed/7G2ZnfExRXI" title="test"></iframe>

            <div class="titlesButtonContainer">
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Learn More </a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Windows</a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Mac</a>
            </div>
          
        </div>

        <div>
            
            <h2>Gundam VS Maxiboost ON</h2>
            <iframe width="550" height="400"src="https://www.youtube.com/embed/WBvYIGzos2w" title="test"></iframe>

            <div class="titlesButtonContainer">
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Learn More</a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Windows</a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Mac</a>
            </div>

        </div>

        <div>
            
            <h2>Gundam Full Extreme VS</h2>
            <iframe width="550" height="400"src="https://www.youtube.com/embed/5rCLBgB3mnQ" title="test"></iframe>

            <div class="titlesButtonContainer">
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Learn More</a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Windows</a>
                <a href="https://gundam.fandom.com/wiki/Gundam_Versus" class="titles-btn">Download for Mac</a>
            </div>

          
        </div>

    </div>

</div>

<script>
    
    var titlesButtons = document.querySelectorAll('.titlesButtonContainer a');

    titlesButtons.forEach(button => {
    button.addEventListener('click', function (event) {  //When button is clicked, add the clicking animation and remove it after a delay
    event.preventDefault();
    button.classList.add('clicked');   

    setTimeout(() => {
        button.classList.remove('clicked');
        }, 5000); 
    });
    });
    
</script>

</html>



