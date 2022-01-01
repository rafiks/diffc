<script>
    import PatientDemo from "./PatientDemo.svelte";
    import Instrument from "./Instrument.svelte";
    import ManDiff from "./ManDiff.svelte";
    import Morphology from "./Morphology.svelte";
</script>

<h1>Manual Differential Cell Counter</h1>

<PatientDemo />
<Instrument />
<ManDiff />
<Morphology />

<style>
    h1 {
        text-align: center;
    }
</style>
