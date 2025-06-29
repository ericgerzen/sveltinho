<script>
    import { onMount } from 'svelte';

    onMount(() => {
        document.title = "PC Hardware Deals";
    });
</script>

<section class="tall-section">
    <div class="left-content">
        <h1 class="text-3xl">Encontrá las mejores ofertas para componentes de computadora.</h1>
    </div>
    <div class="image-grid">
        <img src="/pc.png" alt="Pc">
        <img src="/keyboard.png" alt="Keyboard">
        <img src="/wcooling.png" alt="Water Cooling">
        <img src="/gpu.png" alt="GPU">
    </div>
</section>

<style>
    .tall-section {
        background: #5A3C78;
        min-height: 40rem;
        width: 100%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        padding: 0 4vw;
        box-sizing: border-box;
    }
    .left-content {
        flex: 1 1 40%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
    }
    .tall-section h1 {
        font-family: 'Crete Round', serif;
        font-size: 4rem;
        color: white;
        margin: 0;
    }
    .image-grid {
        flex: 1 1 60%;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        column-gap: 2vw;
        row-gap: 0;
        max-width: 40vw;
        max-height: 40vw;
        width: 100%;
        height: 100%;
        justify-items: center;
        align-items: center;
        align-self: center;
        margin: 0;
        box-sizing: border-box;
    }
    .image-grid img {
        width: 100%;
        max-width: 20vw;
        height: auto;
        max-height: 20vw;
        object-fit: contain;
        border-radius: 0.5rem;
        background: #fff2;
        box-shadow: 0 2px 8px #0002;
        transition: transform 0.2s;
        display: block;
    }
    .image-grid img:hover {
        transform: scale(1.05);
    }
    @media (max-width: 900px) {
        .tall-section {
            flex-direction: column;
            align-items: flex-start;
        }
        .image-grid {
            max-width: 90vw;
            max-height: none;
        }
        .image-grid img {
            max-width: 40vw;
        }
    }
</style>