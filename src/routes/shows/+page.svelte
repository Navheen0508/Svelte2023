<div class="mainIndexContainer">

    <div class="mainIndexHeader">
        
        <div class="headerImages">
            
            <img class="containImg indexLogoImg" src="../img/indexlogo.png" alt="title icon">
        
        </div>

        <div class ="mainIndexButtonsContainer">
            
            <a href="routes/page"><button class="indexNavigationButtons">Mobile Suits</button></a>
            <button class="indexNavigationButtons">Titles</button>
            <button class="indexNavigationButtons">Shows</button>
            <a href="about"><button class="indexNavigationButtons">About</button></a>

        </div>

        
        
    
    </div>

    <div class="showVideoContainer">

        <video src="../video/gun1intro.mp4" class="vSlider" loop controls>
                
            <track kind="captions">
        
        </video>

        <ul>
            <li onclick="videoslider('../video/gun1intro.mp4')"><video src="../video/gun1intro.mp4" class="vSlider" loop controls> <track kind="captions"> </video></li>
            <li onclick="videoslider('../video/gun2intro.mp4')"><video src="../video/gun2intro.mp4" class="vSlider" loop controls> <track kind="captions"> </video></li>
            <li onclick="videoslider('../video/gun3intro.mp4')"><video src="../video/gun3intro.mp4" class="vSlider" loop controls> <track kind="captions"> </video></li>
            <li onclick="videoslider('../video/gun4intro.mp4')"><video src="../video/gun4intro.mp4" class="vSlider" loop controls> <track kind="captions"> </video></li>


        </ul>
            
    </div>

    <div class="footerDiv">

        Texting text

    </div>

</div>

<script>
        function videoslider(links){
            document.querySelector(".vSlider").src = links;
        }
</script>