<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import MoneyIcon from './icons/MoneyIcon.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import IconPositive from './icons/IconPositive.vue'
import PercentIcon from './icons/PercentIcon.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <IconPositive />
    </template>
    <template #heading> Legalização de Empresas</template>
    <p> Abra, altere, regularize e faça o encerramento de empresas em poucos dias, sem sair de casa. </p>    

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/paper.svg" width="30" height="30" alt=""> -->
      <MoneyIcon />

    </template>
    <template #heading>Declaração de IRPF, IRPJ e ITR</template>
    <p>Não corra riscos de pagar multas e tenha mais tranquilidade ao realizar a sua declaração. Identificamos a melhor forma de economizar no pagamento de impostos.</p>
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/query.svg" height="30" width="30" alt="planejamento"> -->
      <DocumentationIcon />
    </template>
    <template #heading>Planejamento Tributário</template>

    <p>Sua empresa está pagando mais impostos do que deveria? Por meio dessa ferramenta, conhecida como elisão fiscal, diminuímos o pagamento de tributos de forma lícita. O contribuinte tem o direito de estruturar o seu negócio da maneira que melhor lhe pareça, procurando a diminuição dos custos de seu empreendimento, inclusive dos impostos.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/group.svg" height="30" width="30" alt="assessoria"> -->
     <CommunityIcon />

    </template>
    <template #heading>Contabilidade Consultiva</template>
      <p>Nessa área da contabilidade, o contador atua muito mais próximo dos clientes e de maneira estratégica, auxiliando na tomada de decisão de forma racional e planejada.</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/group.svg" height="30" width="30" alt="assessoria"> -->
      <ToolingIcon />
    </template>
    <template #heading> Profissional liberal</template>
      <p>Faça a regularização do seu negócio e desenvolva sua atividade com segurança e pagando seus impostos da maneira correta. Trabalhamos com Psicólogos, Veterinários, Nutricionistas, Arquitetos, Advogados, Engenheiros, Médicos entre outros
      </p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <!-- <img src="src/assets/calculate.svg" height="30" width="30" alt="cálculos"> -->
      <PercentIcon />
      
    </template>
    <template #heading> Cálculos para Advogados</template>
<p>
  Para realizar cálculos judiciais se faz necessário uma leitura minuciosa dos documentos, verificação de índices de correção, juros de mora, base de cálculo, entre outros detalhes. Nesse sentido, uma parceria com um perito contador pode proporcionar maior economia de tempo e esforço, além de contribuir com seus resultados na advocacia.
</p>
    
  </WelcomeItem>
</template>
