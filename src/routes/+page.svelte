<script>

  import {AccessibillityGraph, AutomaticScan, ErrorResult, TypeGraph, Icon} from '$lib'
  export let data = data;
  export let company = data.sites;
  export let result = data.scans[0];
  export let resultsheet = data.scans;
</script>

<main class="wrapper">
  
  <AutomaticScan {result} />
  
  <ErrorResult {result} {Icon} />
  
  <TypeGraph {result}/>

  <AccessibillityGraph {resultsheet}/>
</main>

<footer>
</footer>

<style>
  .wrapper {
    margin: auto;
    max-width: 1100px;
  }



  main {
    display: grid;
    grid-template-columns: 2.2fr 0.8fr; 
    grid-template-rows: 1fr 1fr 1.2fr;   
    gap: 20px;  
    height: 90%;
    margin: 20px auto;
  }

  @media only screen and (max-width: 1600px) {

    .wrapper{
      max-width: 900px;
    }

    main {
    display: flex;
    flex-direction: column;
  }
  
}

</style>