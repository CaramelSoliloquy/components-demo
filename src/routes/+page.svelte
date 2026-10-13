<script>
    import Card from '$lib/components/Card.svelte';
    let people = [
        {
            fullName:"Phill Connors",
            favouriteSong:"I got You Babe",
            petsName: "Punxsutawney Phil"
        },
        {
            fullName:"Louis Loaf",
            favouriteSong:"Gimme Gimme Gimme",
            petsName: "Pea"
        },
        {
            fullName:"ManMan the Third",
            favouriteSong:"Toxic",
            petsName: "Manly Birb"
        },        
        {
            fullName:"Meow",
            favouriteSong:"Im gato",
            petsName: "meowp"
        },
    ];
</script>

<main>
    {#each people as person}
        <Card bananas={person}/>
    {/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>