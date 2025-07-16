<script lang="ts">
import type IReceita from '@/interfaces/IReceita';
import type { PropType } from 'vue';

export default {
  props: {
    receita: { type: Object as PropType<IReceita>, 
    required: true }
  },
  emits: ['editarReceitas']
}
</script>

<template>
    <article class="receita">
        <header class="receita__cabecalho">            
            <img class="receita__imagem" :src="`/imagens/receitas/${receita.imagem}`" :alt="`Foto de ${receita.nome}`">
        </header>

        <section class="receita__corpo">
            <h2 class="paragrafo receita__nome">{{ receita.nome }}</h2>
        </section>
    </article>
</template>

<style scoped>
.receita {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  width: 19.5rem;
  padding: 1rem;
  border-radius: 1rem;
  background: var(--branco, #FFF);
  box-shadow: 4px 4px 10px 0px rgba(68, 68, 68, 0.05);
}

.receita__cabecalho {
  display: flex;
  justify-content: center;
}

.receita__imagem {
  width: 100%;
}

.receita__corpo {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>