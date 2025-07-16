<template>
    <footer class="rodape">
        <p class="texto-rodape">
            Desenvolvido por
            <a href="#" class="link-rodape">
                Nekimiau | 2025  
            </a>            
        </p>
    </footer>    
</template>

<style scoped>
.rodape {
    background-color: var(--verde-medio, #3D6D4A);
    color: var(--creme, #FFFAF3);
    padding: 1rem;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
}
.texto-rodape {
    margin: 0;
    font-size: 0.875rem;
    color: var(--creme, #FFFAF3);
}
.link-rodape {
    color: var(--coral, #F0633C);
    text-decoration: none;
}
.link-rodape:hover {
    text-decoration: underline;
}
</style>