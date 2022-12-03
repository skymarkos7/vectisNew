<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading> Legalização de Empresas</template>
    <p> Abra, altere, regularize e faça o encerramento de empresas em poucos dias, sem sair de casa. </p>    

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/paper.svg" width="30" height="30" alt=""> -->
    </template>
    <template #heading>Declaração de IRPF, IRPJ e ITR</template>
    <p>Por meio dessa ferramenta, conhecida como elisão fiscal, diminuímos o pagamento de tributos de forma lícita. O contribuinte tem o direito de estruturar o seu negócio da maneira que melhor lhe pareça, procurando a diminuição dos custos de seu empreendimento, inclusive dos impostos.</p>
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/query.svg" height="30" width="30" alt="planejamento"> -->
    </template>
    <template #heading>Planejamento Tributário</template>

    <p>Identificamos a melhor forma de economizar no pagamento de impostos.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/group.svg" height="30" width="30" alt="assessoria"> -->
    </template>
    <template #heading>Contabilidade Consultiva</template>
      <p>Nessa área da contabilidade, o contador atua muito mais próximo dos clientes e de maneira estratégica, auxiliando na tomada de decisão de forma racional e planejada.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/group.svg" height="30" width="30" alt="assessoria"> -->
    </template>
    <template #heading> Cálculos para Profissional liberal</template>
      <p>Faça a regularização do seu negócio e desenvolva sua atividade com segurança e pagando seus impostos da maneira correta. Trabalhamos com Psicólogos, Veterinários, Nutricionistas, Arquitetos, Advogados, Engenheiros, Médicos entre outros
      </p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/calculate.svg" height="30" width="30" alt="cálculos"> -->
    </template>
    <template #heading> Cálculos para Advogados</template>

    As an independent project, Vue relies on community backing for its sustainability. You can help
    us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </WelcomeItem>
</template>
