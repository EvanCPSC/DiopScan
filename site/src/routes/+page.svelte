<script lang="ts">
	import diopscanLogo from '#lib/assets/diopscan.svg';
    import diopscanHero from '#lib/assets/diopscanhero.png';
    import Navbar from '#lib/components/Navbar.svelte';
    import Footer from '#lib/components/Footer.svelte';
</script>

<Navbar />

<main>
    <div class="hero">
        <div class="hero-left">
            <h1>A new perspective on medical imaging research.</h1>
            <p>Exploring how machine learning can help identify potential signs of cancer in medical images and support a more informed path to clinical review.</p>
        </div>
        <div class="hero-right">
            <img src={diopscanHero} alt="DiopScan Hero" />
        </div>
    </div>
    <div class="technologies">
        <h2>Technologies</h2>
        <div class="cards">
            <div class="card">
                <h3>Lorem Ipsum</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dictum sem ac sagittis blandit. Sed eleifend molestie tincidunt. Vestibulum at elit orci. Proin iaculis, orci.</p>
            </div>
            <div class="card">
                <h3>Lorem Ipsum</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dictum sem ac sagittis blandit. Sed eleifend molestie tincidunt. Vestibulum at elit orci. Proin iaculis, orci.</p>
            </div>
            <div class="card">
                <h3>Lorem Ipsum</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dictum sem ac sagittis blandit. Sed eleifend molestie tincidunt. Vestibulum at elit orci. Proin iaculis, orci.</p>
            </div>
        </div>
    </div>
</main>

<Footer />

<style>
    .hero {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 2rem;
        background-color: var(--primary-bg);
    }
    .hero-left {
        flex: 1;
        padding-right: 2rem;
        h1 {
            font-size: 2.2rem;
            font-family: "Roboto Slab", serif;
        }
    }
    .hero-right {
        flex: 1;
        display: flex;
        justify-content: center;
        img {
            max-width: 90%;
            height: auto;
        }
    }
    .technologies {
        padding: 2rem;
        padding-bottom: 5rem;
        background-color: white;
        h2 {
            font-size: 1.8rem;
            font-family: "Roboto Slab", serif;
            margin-bottom: 3rem;
        }
    }
    .cards {
        display: flex;
        gap: 1rem;
        width: 90%;
        margin: auto;
    }
    .card {
        flex: 1;
        padding: 1rem;
        background-color: var(--primary-bg);
        border: 1px solid var(--shadow-color);
        border-radius: 8px;
        box-shadow: 0 2px 4px var(--shadow-color);
    }
</style>