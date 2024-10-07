<script>
  import {Title, AccessibillityGraph, AutomaticScan, ErrorResult, TypeGraph, Icon} from '$lib'
  export let data = data;
  export let company = data.sites;
  export let result = data.scans[0];
  export let resultsheet = data.scans;
</script>

<Title { company }/>
  
<AutomaticScan {result} />

<ErrorResult {result} {Icon} />

<TypeGraph {result}/>

<AccessibillityGraph {resultsheet}/>