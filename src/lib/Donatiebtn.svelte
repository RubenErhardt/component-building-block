<button popovertarget="donation" popovertargetaction="show" class="donation-button">
    <img src="./4128927.png" alt="Doneren" class="button-icon">Doneren
</button>

<div popover="auto" id="donation" class="popup">
    <button popovertarget="donation" popovertargetaction="hide" class="close-button" aria-label="Sluit">X</button>
    <h2>Doneren</h2>
    <p>Wij bieden jonge, aspirerende journalisten een podium en begeleiding. Dat kunnen we nog beter met jouw steun. Die steun komt met twee voor de prijs van een, want onze sponsor matcht jouw donatie, Geef jij ons vijf euro? Dan ontvangen wij een tientje.</p>
    <fieldset>
        <div class="amount-options">
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
        </div>

        <label for="amount-other" class="other">
            <input type="radio" id="amount-other" name="donation" value="other"> Ander bedrag:
        </label>
    </fieldset>
</div>

<style>
    h2 {
        font-weight: bolder;
        margin-top: -5px;
        margin-bottom: 10px;
        font-size: 42px;
    }

    p {
        color: #6b6b6b;
        margin-bottom: 20px;
    }

    fieldset {
        all: unset;
        padding: 0;
        font-weight: bolder;
    }

    .popup {
        background-color: #f2f2f2;
        outline: 1px solid black;
        width: 440px;
        overflow: hidden;
        height: 260px;
        position: relative;
        padding: 50px;
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

    input[type="radio"] {
        position: absolute;
        opacity: 0;
        pointer-events: none;
    }

    .button-icon {
        width: 20px;
        height: auto;
        margin-right: 8px;
    }

    .donation-button:focus-visible {
        outline: 2px solid #000000;
    }

    .amount-options {
        display: flex;
        justify-content: space-between;
        gap: 10px; 
        margin-bottom: 10px; 
    }

    .amount-options label{
        width: 95px;
    }

    label {
        display: inline-block;
        padding: 8px 16px;
        background-color: #fff;
        color: #000;
        border: 2px solid #000;
        font-size: 16px;
        cursor: pointer;
        text-align: center;
        transition: all 0.3s ease;
    }

    label:hover,
    label:focus-within {
        background-color: #000000;
        color: white;
    }

    .other {
        width: 405px;
        height: 20px;
    }

    .close-button {
        position: absolute;
        top: 10px;
        right: 10px;
        background-color: transparent;
        border: none;
        font-size: 20px;
        color: #000;
        cursor: pointer;
        padding: 5px;
        z-index: 10;
    }

    .close-button:hover {
        color: #E85340;
    }
</style>
