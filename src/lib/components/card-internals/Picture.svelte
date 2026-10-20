<script>
    import billm from '$lib/assets/images/groundhog-day.webp';
    import meow from '$lib/assets/images/OIP.webp';
    let { oranges = { img:billm, alt: meowps} } = $props();
</script>

<img src="{oranges.img}" alt="{oranges.alt}">

<style>
    img {
            width: 200px;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: center;
            border-radius: 30px;
            corner-shape: circle;
        }
</style>