<main>
<button popovertarget="popover-one" class="btn-primary">open popup</button>

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
    </div>
</main>

<style>
    
</style>
