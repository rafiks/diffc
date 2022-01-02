<script>
    import PatientDemo from "./PatientDemo.svelte";
    import Instrument from "./Instrument.svelte";
    import ManDiff from "./ManDiff.svelte";
    import Morphology from "./Morphology.svelte";
</script>

<div bp="grid"><h1>Manual Differential Cell Counter</h1></div>
<PatientDemo />
<div bp="grid4">
    <Instrument />
    <ManDiff />
    <Morphology />
</div>

<style>
    /* h1 {
    text-align: center;
    } */
</style>
