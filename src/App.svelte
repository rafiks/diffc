<script>
    import PatientDemo from "./PatientDemo.svelte";
    import Instrument from "./Instrument.svelte";
    import ManDiff from "./ManDiff.svelte";
    import Morphology from "./Morphology.svelte";
</script>

<div bp="grid 12" class="title"><h1>Manual Differential Cell Counter</h1></div>
<PatientDemo />
<div bp="grid 4">
    <div><Instrument /></div>
    <div><ManDiff /></div>
    <div><Morphology /></div>
</div>

<style>
    .title {
        background-color: rgba(88, 150, 88, 50);
    }
    div {
        background-color: bisque;
        margin: 0;
    }

    /* h1 {
    text-align: center;
    } */
</style>
