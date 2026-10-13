<script>
    let { apples = {
    fullName:"meow",
    favouriteSong:"meow",
    petsName: "meow"
    }   } = $props();
</script>

<section>
    <h2>{apples.fullName}</h2>
    <dl>
        <dt>Favourite song:</dt>
        <dd>{apples.favouriteSong}</dd>
        <dt>Pet's name:</dt>
        <dd>{apples.petsName}</dd>
    </dl>
</section>

<style>
    dl {
        display: grid;
        grid-template-columns: max-content 1fr;
        gap: 0.5rem 1rem;
    }

    dt {
        font-weight: bold;
    }

    dd {
        margin: 0;
    }
</style>