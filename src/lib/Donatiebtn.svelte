
<!-- <button popovertarget="popover-one" class="btn-primary">open popup</button>

    <div class="overlay" id="popover-one" popover="auto">
    <button class="btn-close" popovertarget="popover-one" popovertargetaction="hide">X</button>

    <p>Doneren</p>
    <div>
        <label for="amount-10">
            <input type="radio" id="amount-10" name="donation" value="10">
            10 Euro
        </label>
    </div>
    <div>
        <label for="amount-25">
            <input type="radio" id="amount-25" name="donation" value="25">
            25 Euro
        </label>
    </div>
    <div>
        <label for="amount-other">
            <input type="radio" id="amount-other" name="donation" value="other">
            Ander bedrag:
            <input type="number" id="custom-amount" name="custom-amount" min="1" placeholder="Voer een bedrag in">
        </label>
    </div>
    </div> -->

    <button popovertarget="donation" popovertargetaction="show" class="donation-button">
        <img src="./4128927.png" alt="Doneren" class="button-icon">
        Doneren
    </button>
    
    <article popover="auto" id="donation">
        <button popovertarget="donation" popovertargetaction="hide" class="close-button">X</button>
        <h2>Doneren</h2>
        <p>Wij bieden jonge, aspirerende journalisten een podium en begeleiding. Dat kunnen we nog beter met jouw steun. Die steun komt met twee voor de prijs van een, want onze sponsor matcht jouw donatie, Geef jij ons vijf euro? Dan ontvangen wij een tientje.</p>
        <label for="amount-10">
            <input type="radio" id="amount-10" name="donation" value="10">
            €10
        </label>
    
        <label for="amount-25">
            <input type="radio" id="amount-25" name="donation" value="25">
            €25
        </label>
    
        <label for="amount-50">
            <input type="radio" id="amount-50" name="donation" value="50">
            €50
        </label>
    
        <label for="amount-other" class="other">
            <input type="radio" id="amount-other" name="donation" value="other">
            Ander bedrag:
            <input type="number" id="custom-amount" name="custom-amount" min="1" placeholder="Voer een bedrag in">
        </label>
    </article>
    
<style>
h2{
    font-weight: bolder;
    margin-top: -10px;
    margin-bottom: -5px;
    font-size: 42px;
}

p{
    color: #6b6b6b;
}

article{
    background-color: #f2f2f2;
    outline: 1px solid black;
    width: 360px;
    overflow: hidden;
    height: 230px;
    position: relative;
    padding: 40px;
}
.donation-button {
    all: unset;
    --btn-color: #E85340;
    --btn-text: #ffffff;
    background-color: var(--btn-color);
    border-radius: 2px;
    color: var(--btn-text);
    cursor: pointer;
    display: flex; 
    align-items: center; 
    padding: 8px 12px; 
}

.button-icon {
    width: 20px; 
    height: auto;
    margin-right: 8px; 
}

.donation-button:focus-visible {
    outline: 2px solid #000000;
}

/* Verberg de standaard radiobutton en maak ruimte voor de aangepaste stijl */
input[type="radio"] {
    display: none; /* Verberg de standaard radiobutton */
}

label {
    display: inline-block;
    padding: 8px 16px;
    width: 21%;
    margin-bottom: 10px;
    background-color: #fff; 
    color: #000;
    border: 2px solid #000; 
    font-size: 16px;
    cursor: pointer;
    transition: all 0.3s ease; 
}

/* Stijl bij hover */
label:hover {
    background-color: #000000;
    color: white;
}


/* Specifieke stijl voor de input met een ander bedrag */
input[type="number"] {
    margin-left: 10px; /* Ruimte tussen het tekstveld en de radiobutton */
    padding: 5px;
    border-radius: 4px;
    border: 1px solid #ccc;
}

/* Stijl voor de close-button */
.close-button {
    position: absolute; /* Dit plaatst de knop absoluut binnen het artikel */
    top: 10px; /* 10px van de bovenkant van het artikel */
    right: 10px; /* 10px van de rechterkant van het artikel */
    background-color: transparent; /* Transparante achtergrond voor de knop */
    border: none; /* Verwijder de standaard knop rand */
    font-size: 20px; /* Maak de tekst groot genoeg voor de 'X' */
    color: #000; /* Zwarte tekstkleur */
    cursor: pointer; /* Cursor verandert naar handje */
    padding: 5px; /* Kleine padding voor de knop */
    z-index: 10; /* Zorg ervoor dat de knop boven andere elementen komt */
}

/* Optioneel: stijl de knop bij hover */
.close-button:hover {
    color: #E85340; /* Verander de kleur naar oranje-rood bij hover */
}

.other{
    width: 86%;
    height: 20px;
}



</style>
