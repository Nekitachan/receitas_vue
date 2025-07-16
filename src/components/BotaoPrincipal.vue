<script lang="ts">
export default {
  props: {
    texto: { type: String, required: true },
  }
}
</script>

<template>
    <section>        
        <button class="paragrafo-lg botao-principal">
          {{ texto }}
        </button>
    </section> 
</template>

<style scoped>
.botao-principal {
    background-color: var(--coral, #F0633C);
    color: var(--creme, #FFFAF3);
    border: none;
    padding: 1rem 2rem;
    border-radius: 2rem;
    font-size: 1rem;
    font-weight: 700;
    cursor: pointer;
    transition: background-color 0.3s ease;
    box-shadow: 4px 4px 15px 0px rgba(255, 115, 76, 0.25);
    transition: 0.2s;
    display: flex;
    justify-content: center;
    align-items: center;
}
.botao-principal:hover {
    background-color: var(--coral-hover, #D04F2B);
}
.botao-principal:focus {
    outline: none;
}
</style> 