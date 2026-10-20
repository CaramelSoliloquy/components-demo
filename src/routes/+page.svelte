<script>
    import Card from '$lib/components/Card.svelte';
    import billm from '$lib/assets/images/groundhog-day.webp';
    import meow from '$lib/assets/images/OIP.webp';
    let { data } = $props(); // Must call it "data" to get it from the +page.js fetch
    let userlist = data.users.users;
    let people = [
        {
            fullName:"Phill Connors",
            favouriteSong:"I got You Babe",
            petsName: "Punxsutawney Phil",
            img:billm,
            alt:"Phill Connors"
        },
        {
            fullName:"Louis Loaf",
            favouriteSong:"Gimme Gimme Gimme",
            petsName: "Pea",
            img:meow,
            alt: "Louis Loaf"
        },
        {
            fullName:"ManMan the Third",
            favouriteSong:"Toxic",
            petsName: "Manly Birb",
            img:billm,
            alt:"Phill Connors"
        },        
        {
            fullName:"Meow",
            favouriteSong:"Im gato",
            petsName: "meowp",
            img:billm,
            alt:"Phill Connors"
        }
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