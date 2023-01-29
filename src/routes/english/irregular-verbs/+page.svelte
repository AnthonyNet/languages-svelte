<script>
    import Navbar from '../../../components/navbar/Navbar.svelte';
    import Irregular from '../../../components/irregular/Irregular.svelte';
    import {IrregularVerbs} from '../../../myData/index.js';
</script>

<Navbar />
<Irregular myData={IrregularVerbs} />