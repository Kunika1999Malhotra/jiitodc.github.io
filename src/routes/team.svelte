<svelte:head>
  <title>Team</title>
</svelte:head>

<script>
  import { onMount } from 'svelte';

  import TeamComponent from '../components/TeamComponent.svelte';

  import AOS from 'aos';
  import 'aos/dist/aos.css';
  import 'aos/dist/aos.js';

  import 'lazysizes';
  import 'lazysizes/plugins/parent-fit/ls.parent-fit';

  onMount(() => {
    AOS.init();
  })
</script>

<div class="main-title">TEAM</div>

<section class="card-list">
  <TeamComponent imgSrc="Photos/Poster.png" name="Aayush Sahu" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
  <TeamComponent imgSrc="Photos/Poster.png" name="Aachman Mittal" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
  <TeamComponent imgSrc="Photos/Poster.png" name="Aaryan Porwal" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
  <TeamComponent imgSrc="Photos/Poster.png" name="Akshat Agarwal" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
  <TeamComponent imgSrc="Photos/Poster.png" name="Ishan" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
  <TeamComponent imgSrc="Photos/Poster.png" name="Rudraksh Pareek" role="Core Member"
    gitLink="https://www.github.com/aayushmau5" />
</section>

<style>
  .main-title {
    font-size: 3rem;
    font-weight: bold;
    text-align: center;
    padding-bottom: 1rem;
    border-bottom: 2px solid #ff8c00;
  }

  .card-list {
    display:grid;
    grid-template-columns: repeat(2,1fr);
    gap:7rem 3rem;
  }

  @media (max-width:700px) {
    .main-title {
      font-size:2.5rem;
    }
    .card-list {
      grid-template-columns: 1fr;
      gap:2rem 1rem;
    }
  }
</style>
