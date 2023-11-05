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

        <video src="../video/gun1intro.mp4" class="vSlider" poster="../img/gun1th.JPG" autoplay controls>
                
            <track kind="captions">
        
        </video>

        <ul>
            <li onclick="videoslider('video1','../video/gun1intro.mp4')">

                <video id="video1" src="../video/gun1intro.mp4" class="vSlider" poster="../img/gun1th.JPG" controls> 

                    <track kind="captions"> 

                </video>
            
            </li>

            <li onclick="videoslider('video2','../video/gun2intro.mp4')">

                <video id="video2" src="../video/gun2intro.mp4" class="vSlider" poster="../img/gun2th.JPG" controls> 

                    <track kind="captions"> 

                </video>

            </li>

            <li onclick="videoslider('video3','../video/gun3intro.mp4')">

                <video id="video3" src="../video/gun3intro.mp4" class="vSlider" poster="../img/gun3th.JPG" controls> 

                    <track kind="captions"> 

                </video>
            </li>

            <li onclick="videoslider('video4','../video/gun4intro.mp4')">

                <video id="video4" src="../video/gun4intro.mp4" class="vSlider" poster="../img/gun4th.JPG" controls> 

                    <track kind="captions"> 

                </video>

            </li>

            <li onclick="videoslider('video5','../video/gun5intro.mp4')">

                <video id="video5" src="../video/gun5intro.mp4" class="vSlider" poster="../img/gun5th.JPG" controls> 

                    <track kind="captions"> 

                </video>
                
            </li>


        </ul>
            
    </div>

    <div class="footerDiv">

        

    </div>

</div>


<script>
    
    function videoslider(links) {
    const vSlider = document.querySelector(".vSlider");
    vSlider.src = links;
    vSlider.play(); // Autoplay the new video
}
</script>