<script>
    import Keylog from "./Keylog.svelte";
    import Total from "./Total.svelte";

    let key;
    let total_cells = 0;
    let segs = 0;
    let lymp = 0;
    let mono = 0;
    let eosi = 0;
    let baso = 0;
    // count the total base on the number
    console.log(total_cells);

    //
    //
    function counter_d(event) {
        key = event.key;
        console.log(key);

        if (total_cells < 100) {
            if (key == "e") {
                total_cells += 1;
                segs += 1;
            } else if (key == "u") {
                total_cells += 1;
                lymp += 1;
            } else if (key == "o") {
                total_cells += 1;
                mono += 1;
            } else if (key == "j") {
                total_cells += 1;
                eosi += 1;
            } else if (key == "k") {
                total_cells += 1;
                baso += 1;
            }
        }
    }

    class Cbc {}
    class Seg {}

    class Lym {}
    class Mono {}
    class Eos {}
    class Baso {}
</script>

<svelte:window on:keydown={counter_d} />
<div bp="grid 12">
    <p>Manual Differential</p>
    <p>Total = {total_cells}</p>
    <div>Segs = {segs}</div>
    <div>Lymp = {lymp}</div>
    <div>
        <ul>
            <li th />
            <li />
            <li />
            <li />
            <li />
        </ul>
    </div>
</div>

<Keylog />
<Total />
