<template>
    <div class="container">
        <section class="sobre">
            <h2>Sobre a Truckme</h2>
            <p>A TRUCK ME é uma empresa inovadora que transforma a maneira como serviços de transporte são gerenciados e realizados. Através da nossa avançada Plataforma Web, garantimos que todos os requisitos e obrigações de uma transportadora tradicional sejam rigorosamente cumpridos, proporcionando um serviço confiável e eficiente.</p>

            <p>Nosso objetivo é conectar embarcadores aos transportadores autônomos mais qualificados, criando um elo forte e eficiente na cadeia de logística. Utilizamos um criterioso processo de gestão para selecionar os melhores profissionais, assegurando que nossos clientes recebam sempre o melhor serviço possível.</p>

            <p>Além disso, a TRUCK ME simplifica todos os processos relacionados ao frete, desde a contratação até a execução, tornando a experiência de transporte mais rápida, transparente e segura para todas as partes envolvidas.</p>

            <p>Na TRUCK ME, acreditamos que a tecnologia pode revolucionar o setor de transporte, e estamos comprometidos em fornecer soluções que otimizem a eficiência e a confiabilidade dos serviços de frete. Seja você um embarcador buscando serviços de transporte de qualidade ou um transportador autônomo em busca de novas oportunidades, a TRUCK ME é a parceira ideal para suas necessidades logísticas.</p>

            <button class="saiba" id="saibaMais" @click="toggleInfo">Saiba mais!<i class="fa-solid fa-arrow-down"></i></button>
        </section><!--sobre-->

        <section class="saiba-mais" id="infoSessao" :class="{ show: isShown }">
            <div class="saiba-mais-text">
                <h2>Saiba Mais sobre a TRUCK ME</h2>

                <h4>Nossa Missão</h4>
                <p>Na TRUCK ME, estamos comprometidos em revolucionar o setor de transporte. Nosso objetivo é fornecer soluções tecnológicas que simplificam e otimizam todos os processos logísticos, desde a contratação até a execução do frete.</p>

                <h4>Plataforma Avançada</h4>
                <p>Nossa plataforma web é o coração da nossa operação. Com ela, conectamos embarcadores a transportadores autônomos altamente qualificados, garantindo que cada transporte seja realizado de forma eficiente e segura. A plataforma oferece uma interface intuitiva e funcionalidades robustas, permitindo uma gestão completa e transparente de todas as operações de transporte.</p>

                <h4>Conformidade e Confiabilidade</h4>
                <p>Cumprir todos os requisitos e obrigações de uma transportadora tradicional é uma prioridade para nós. Garantimos que todas as normas e regulamentações sejam rigorosamente seguidas, proporcionando tranquilidade e segurança para nossos clientes e parceiros.</p>

                <h4>Para Quem é a TRUCKME</h4>
                <p>Se você é um embarcador procurando por serviços de transporte confiáveis e eficientes, ou um transportador autônomo em busca de novas oportunidades, a TRUCK ME é a parceira ideal para suas necessidades logísticas. Nossa tecnologia e expertise estão à sua disposição para garantir que cada transporte seja um sucesso.</p>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: 'AboutComponent',
    data() {
        return {
            isShown: false
        };
    },
    methods: {
        toggleInfo() {
            this.isShown = !this.isShown;
        }
    }
}
</script>


