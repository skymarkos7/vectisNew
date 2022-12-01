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
    <template #heading>Escrituração Contábil e Fiscal</template>
    <p>Além de ser um documento exigido por lei a Escrituração é complexa e cheia de detalhes e pode gerar muita dor de cabeça, deixe-a com a gente e mantenha o foco no seu negócio.</p>
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/query.svg" height="30" width="30" alt="planejamento"> -->
    </template>
    <template #heading>Planejamento Tributário | Declaração de IRPF, IRPJ e ITR</template>

    <p>Identificamos a melhor forma de economizar no pagamento de impostos.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/group.svg" height="30" width="30" alt="assessoria"> -->
    </template>
    <template #heading>Contabilidade Consultiva  Folha de pagamento para doméstica</template>
      <p>Nessa área da contabilidade, o contador atua muito mais próximo dos clientes e de maneira estratégica, auxiliando na tomada de decisão de forma racional e planejada.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Assessoria Trabalhista e financeira</template>
      <p>É um serviço direcionado aos empregadores, de caráter estritamente técnico, visando propor a adequação
         da atividade empresarial às leis trabalhistas vigentes. Permitindo ao empresário ter mais segurança e
         tranquilidade na gestão dos seus recursos humanos
      </p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/calculate.svg" height="30" width="30" alt="cálculos"> -->
    </template>
    <template #heading> Cálculos para Advogados ou Profissional liberal</template>

    As an independent project, Vue relies on community backing for its sustainability. You can help
    us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </WelcomeItem>
</template>
