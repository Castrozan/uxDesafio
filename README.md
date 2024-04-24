# Entrega - Desaﬁo de usabilidade
-   Lucas de Castro Zanoni

## Análise do Aplicativo Atual:

1. **Dificuldade em encontrar rotas e horários de transporte:**
   - O aplicativo atual apresenta uma dificuldade significativa em encontrar rotas e horários de transporte devido a várias limitações no processo de busca. Uma das principais falhas está na utilização de um único campo para inserção do endereço de partida e destino, o que resulta na ocultação do endereço completo, pois não cabe no campo disponível. Além disso, o aplicativo não oferece recursos de autocomplete ou sugestões automáticas com base nos dados inseridos, tornando a busca mais trabalhosa e suscetível a erros.
   - Essas limitações têm um impacto negativo significativo na experiência do usuário. Primeiramente, a ocultação do endereço completo de partida e destino pode levar a erros na entrada de dados e frustração por parte do usuário ao ter que inserir informações adicionais manualmente.
   - A falta de recursos de autocomplete e sugestões automáticas também aumenta o tempo e o esforço necessários para completar a busca, resultando em uma experiência menos eficiente e mais propensa a erros.

2. **Falta de informações em tempo real:**
   - O problema reside na dispersão e excesso de informações apresentadas de forma desorganizada. As informações sobre a rota estão fragmentadas e mal dispostas, dificultando a identificação e compreensão dos dados para os usuários. A sobrecarga de informações torna a identificação de dados relevantes uma tarefa complexa e confusa.
   - O mapa interativo oferece apenas uma experiência visual sem a funcionalidade de acompanhar os veículos em tempo real. Os usuários não têm a capacidade de visualizar os veículos da rota e sua posição atual, o que limita significativamente a utilidade do mapa para o acompanhamento e planejamento das viagens. Esta falta de interatividade reduz a eficácia do aplicativo em fornecer informações em tempo real e pode levar a uma experiência menos satisfatória para os usuários.

3. **Reorganização dos Menus:**
   - As configurações do aplicativo atual apresentam diversas deficiências que prejudicam a experiência do usuário. Uma das principais falhas é a falta de organização e agrupamento adequados das opções de configuração, resultando em uma interface confusa e desordenada. 
   - A falta de opções de personalização abrangentes também pode levar os usuários a sentirem que o aplicativo não atende às suas necessidades individuais, resultando em uma experiência menos satisfatória e menos propensa a retenção de usuários.

4. **Interface confusa e excesso de opções:**
   - A interface atual é confusa e sobrecarregada, com excesso de opções que podem dificultar a navegação para os usuários.
   - Isso pode causar confusão e frustração, levando os usuários a abandonarem o aplicativo em busca de alternativas mais simples e intuitivas.


## Personas e Mapa de Empatia:

**Persona 1: Estudante Trabalhador**

- **Nome:** Lucas Oliveira
- **Sexo:** Masculino
- **Idade:** 26 anos
- **Profissão:** Estudante e Estagiário em uma Empresa de Tecnologia
- **Cenário:**
  Lucas é um estudante universitário que trabalha como estagiário em uma empresa de tecnologia durante o dia e frequenta a faculdade à noite. Ele depende do transporte público para se locomover pela cidade, seja para ir ao trabalho ou para a faculdade. Devido ao seu horário apertado, Lucas valoriza a eficiência e a pontualidade do transporte público, pois qualquer atraso pode afetar seu desempenho tanto no trabalho quanto nos estudos. Ele está sempre em movimento e busca por um aplicativo de transporte público que seja intuitivo, forneça informações precisas sobre rotas e horários, e ajude a otimizar seu tempo.

- **Desejos:**
  - Encontrar rotas eficientes que minimizem o tempo de deslocamento entre o trabalho e a faculdade.
  - Ter acesso a informações em tempo real sobre horários de ônibus e possíveis atrasos.
  - Personalizar preferências, como receber notificações sobre alterações nos horários de transporte.
  - Facilidade de uso e uma interface intuitiva que permita uma navegação rápida e sem complicações.

**Persona 2: Senhora Maria**

- **Nome:** Maria Silva
- **Sexo:** Feminino
- **Idade:** 68 anos
- **Profissão:** Aposentada
- **Cenário:**
  Maria é uma senhora idosa que vive sozinha em um bairro tranquilo da cidade. Ela utiliza o transporte público para se locomover pela cidade, seja para ir ao mercado, ao médico ou para visitar amigos e familiares. Como ela não dirige, depende inteiramente do transporte público para suas necessidades diárias de locomoção. Maria é uma usuária frequente do aplicativo de transporte público, pois facilita a sua vida ao fornecer informações sobre rotas, horários e paradas de ônibus. No entanto, ela enfrenta dificuldades em usar o aplicativo devido à sua idade e falta de familiaridade com tecnologia.

- **Desejos:**
  - Encontrar rotas simples e diretas para suas viagens diárias, levando em consideração sua mobilidade reduzida.
  - Acessar informações claras e fáceis de entender sobre horários de ônibus e locais de parada.
  - Uma interface de aplicativo simples e amigável, com botões grandes e legíveis, que facilite a navegação para usuários mais idosos.
  - Receber alertas sobre alterações nos horários de ônibus ou interrupções no serviço para evitar esperas desnecessárias.
  - Sentir-se segura e confiante ao usar o transporte público, sabendo que pode acessar facilmente as informações necessárias através do aplicativo.

### [**Mapa da Empatia**](https://miro.com/app/board/uXjVKQR_0RQ=/?share_link_id=265925154560)

## Propostas de Melhorias na Arquitetura da Informação:

**Propostas de Melhorias na Arquitetura da Informação:**


1. **Dificuldade em encontrar rotas e horários de transporte:**
   - Em vez de um único campo para inserção de endereço de partida e destino, dividir em dois campos separados para garantir que o endereço completo seja visível e facilmente editável pelo usuário.
   - Implementar recursos de autocomplete e sugestões automáticas com base nos dados inseridos pelo usuário, facilitando a entrada de informações e reduzindo o tempo necessário para completar a busca.
   - Criar uma seção de histórico de viagens anteriores para permitir que os usuários acessem rapidamente rotas frequentemente utilizadas, eliminando a necessidade de inserir manualmente os mesmos dados repetidamente.
   - Todas essas funcionalidades exigirão uma nova tela/modal para que toda informação esteja bem distribuída e não polua a tela do usuário.

2. **Falta de informações em tempo real:**
   - Ao identificar a rota desejada, a tela de detalhes da rota pode ser atualizada para incluir informações em tempo real sobre a localização e status dos transportes que a compõe, como horário previsto para chegada, lotação, tráfego, etc. Um algoritmo de inteligencia artificial será utilizado para calcular o tempo estimado para chegada do veículo e deslocamento do usuário até o ponto de encontro.
   - O mapa estará tomando boa parte do fundo da tela, somente com uma aba inferior exibindo as informações da rota. A aba pode ser minimizada para facilitar a interação com o mapa.
   - O mapa deve ser interativo, permitindo que o usuário veja os veículos preferenciais para a rota no mapa. Assim é possível identificar em que posição da cidade o veículo está e se planejar para saída.
   - É importante que seja possível selecionar para que outro veículo seja utilizado para a rota, caso o usuáiro identifique que o próximo esteja muito lotado ou próximo demais.

3. **Reorganização dos Menus:**
   - As opções de configuração serão ser agrupadas em categorias lógicas e relacionadas para facilitar a navegação do usuário. Separações distintas para configurações de conta, preferências de notificação e configurações de privacidade.
   - As opções de configuração mais utilizadas, como preferências de notificação e privacidade, serão destacadas para facilitar o acesso direto.
   - Cada opção de configuração terá ter uma descrição clara e instruções sobre o propósito e o impacto da configuração. Isso ajudará os usuários a compreenderem melhor suas escolhas.
   - Haverá feedback visual imediato ao realizar alterações nas configurações. Confirmações de alterações bem-sucedidas ou mensagens de erro serão exibidas de forma clara para o usuário.
   - O menu de configurações ocupara toda uma tela, com opçoes listadas para grupos de configurações com contextos adequados.

4. **Pouca personalização e falta de sugestões relevantes:**
   - O aplicativo irá gerenciar o histórico de uso e rotas, além de consumir dados de destinos para alimentar uma base de dados de inteligencia artificial.
   - Esse modelo será utilizado para gerenciar e dar sugestões de rotas e trajetos com base no histório de tráfego na região, atraso de veículos e lotação.


## [**Wireframe de Baixa Fidelidade**](https://miro.com/app/board/uXjVKQR1M50=/?share_link_id=81481901958)