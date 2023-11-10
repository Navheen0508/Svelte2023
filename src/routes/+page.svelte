<html lang="test">

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

    <div class="slider">

        <div class="slides">

            <input type="radio" name="radio-btn" id="radio1">
            <input type="radio" name="radio-btn" id="radio2">
            <input type="radio" name="radio-btn" id="radio3">
            <input type="radio" name="radio-btn" id="radio4">

            <div class="slide first">

                <img src="../img/gun1.png" alt="">

            </div>

            <div class="slide">

                <img src="../img/gun4.png" alt="">

            </div>

            <div class="slide">

                <img src="../img/gun3.png" alt="">

            </div>

            <div class="slide">

                <img src="../img/gun2.png" alt="">

            </div>

            <div class="navigation-auto">

                <div class="auto-btn1"></div>
                <div class="auto-btn2"></div>
                <div class="auto-btn"></div>
                <div class="auto-btn1"></div>

            </div>

            <div class="navigation-manual">

                <label for="radio1" class="manual-btn"></label>
                <label for="radio2" class="manual-btn"></label>
                <label for="radio3" class="manual-btn"></label>
                <label for="radio4" class="manual-btn"></label>

            </div>

        </div>

    </div>

</div>

<script type="text/javascript">
    
    document.addEventListener("DOMContentLoaded", function() {

        var counter = sessionStorage.getItem("slideshowCounter") || 1;  //Get the current slideshow counter value from the session storage or set it to 1 if there isn't one
        document.getElementById('radio' + counter).checked = true;
        var intervalId;                                                 //Store interval ID for slideshow 

        function startSlideshow() {

            clearInterval(intervalId);                                                  //Clear existing interval value and set a new one

            intervalId = setInterval(function() {

                document.getElementById('radio' + counter).checked = false;  //Initialize a slideshow on page load, remembering the slide counter in sessionStorage to remember current slide.
                counter++;

                if (counter > 4) {                                                          
                    counter = 1;                                                        
                }

                document.getElementById('radio' + counter).checked = true;
                sessionStorage.setItem("slideshowCounter", counter);

            }, 5000);                                                       //Advance slide every 5 seconds once and when reaching the end, start over again

        }

        startSlideshow();

    });

</script>

</html>











