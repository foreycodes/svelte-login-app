<script>
    import { onMount } from "svelte"; 

    let data; 
    // fetching data from spoonacular
    onMount(async ()=> {
        const res = await fetch("https://api.spoonacular.com/recipes/complexSearch?&apiKey=9f5a00eb2a454d6893455a09e3ef7964")

        const data = await res.json()
        console.log(data)
    })
</script>
<h1>Home</h1>
