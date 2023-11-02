<script type="text/javascript">

    var counter = 1;

        setInterval(function() {

        document.getElementById('radio' + counter).checked = true;
        counter++;

        if (counter > 4) {
        counter = 1;
        }

        }, 5000);
            
</script>


<div class="mainIndexContainer">
    
    <div class="mainIndexHeader">
        
        <div class="headerImages">
            
            <img class="containImg indexLogoImg" src="../img/indexlogo.png" alt="title icon">

            <div class ="mainIndexButtonsContainer">
            
                <button class="indexNavigationButtons">Mobile Suits</button>
                <button class="indexNavigationButtons">Titles</button>
                <button class="indexNavigationButtons">Shows</button>
                <a href="about"><button class="indexNavigationButtons">About</button></a>
        
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

    <div class="footerDiv">


    </div>

</div>









