# Linha do tempo e a estrutura jurídica da Reforma Tributária do Consumo no Brasil

<img width="950" height="542" alt="image" src="https://github.com/user-attachments/assets/d7c18d97-c638-42fa-9632-76311e322977" />

  - EC 18/65 (Riscada): Refere-se à Emenda Constitucional nº 18 de 1965, que criou o modelo tributário antigo baseado no consumo (como o ICM/ICMS e o ISS). Ela está riscada no slide para representar a substituição desse modelo histórico/antigo que durou quase 60 anos.
  - PEC 45 e PEC 110 (Setas indicando o centro): Propostas de Emenda à Constituição que tramitaram na Câmara dos Deputados (PEC 45) e no Senado Federal (PEC 110). Ambas propunham a criação de um Imposto sobre Valor Agregado (IVA). Elas foram fundidas e ajustadas ao longo das negociações.
  - EC 132/23 (Centro): É a Emenda Constitucional nº 132, promulgada em dezembro de 2023. Ela alterou a Constituição Federal para instituir formalmente a Reforma Tributária do Consumo (sistema de IVA Dual: CBS e IBS).
  - Lei Complementar 214/25 e Lei Complementar 227/26: São as leis que regulamentam e detalham o texto da Constituição:
      - A PLP 68/2024 (projeto principal) regulamenta a instituição da CBS, do IBS e do Imposto Seletivo (IS).
      - A PLP 108/2024 trata da gestão e do Comitê Gestor do IBS.
- Regulamento e Sistema Operacional: O nível onde entram as definições de software, APIs de integração, layouts de documentos fiscais eletrônicos (NF-e, NFS-e, CT-e) e parâmetros do sistema de split payment/crédito financeiro.

## Conceitos Importantes sobre a Reforma Tributária

- IVA Dual (Imposto sobre Valor Agregado): O modelo substitui 5 tributos (PIS, COFINS, IPI, ICMS e ISS) por dois impostos principais e um imposto seletivo:
  - CBS (Contribuição sobre Bens e Serviços): Federal (substitui PIS, COFINS e IPI).
  - IBS (Imposto sobre Bens e Serviços): Estadual/Municipal (substitui ICMS e ISS).
  - IS (Imposto Seletivo): Federal ("Imposto do Pecado" para produtos nocivos à saúde ou ao meio ambiente).

- Princípio do Destino: O tributo passa a pertencer ao local onde o bem/serviço é consumido, não mais onde é produzido.
- Não Cumulatividade Plena: O tributo pago nas etapas anteriores gera crédito financeiro imediato para a empresa pagadora, exigindo controle rigoroso de créditos e débitos fiscais.
- Split Payment: Mecanismo operacional em que o valor do imposto é retido/recolhido automaticamente no momento do pagamento eletrônico ou liquidação bancária.

## "Por que reformar o sistema tributário brasileiro?

<img width="962" height="557" alt="image" src="https://github.com/user-attachments/assets/f0db88d1-1bbf-421a-a470-13a785f91272" />

O Brasil não está apenas em desvantagem competitiva internacional, mas figura no topo do ranking mundial dos sistemas tributários mais complexos e burocráticos do planeta.

O Brasil destaca-se em vermelho com um índice de 0,44, posicionado no grupo mais elevado de complexidade mundial (próximo de países como Índia, Bélgica, Colômbia e Itália).

O Impacto no Negócio e na Tecnologia:

A alta complexidade histórica decorre da sobreposição de 5 tributos diferentes (PIS, Cofins, IPI, ICMS e ISS), espalhados entre 27 legislações estaduais e mais de 5.500 legislações municipais.

Para software e operações, isso gerava o "Custo Brasil": necessidade de regras tributárias dinâmicas gigantescas, tabelas intermináveis de exceções fiscais (ST, regimes especiais) e alto risco de autuação contábil.


## Contexto Legislativo e do Modelo de Governança Dual da Reforma Tributária.

<img width="962" height="532" alt="image" src="https://github.com/user-attachments/assets/60cee26b-917e-47c8-91c0-749d72eff17d" />

### Contexto Legislativo e Base Legal
A Reforma Tributária do Consumo baseia-se na Emenda Constitucional nº 132/2023, que alterou a Constituição Federal para instituir o sistema de IVA Dual. A regulamentação do texto constitucional é feita por Leis Complementares (ex.: LC 214 e LC 227), que definem as regras operacionais, isenções, alíquotas e mecanismos de apuração

 O Modelo de Governança Dual (IVA Dual)
 
O sistema tributário do consumo é dividido em dois grandes pilares de arrecadação e gestão:
- CBS (Contribuição sobre Bens e Serviços) – Âmbito Federal:
    - Órgão Responsável: Receita Federal do Brasil (RFB).
    - Substitui: Tributos federais PIS, COFINS e IPI.
    - Ação: Centralização do recolhimento e fiscalização a nível nacional.
 
- IBS (Imposto sobre Bens e Serviços) – Âmbito Subnacional:
   - Órgão Responsável: Comitê Gestor do IBS (CG-IBS), com representação unificada de Estados e Municípios (COMSEFAZ, CNM, FNP).
   - Substitui: ICMS (27 Estados/DF) e ISS (mais de 5.500 Municípios).
   - Ação: Padronização nacional das regras do imposto, eliminando a fragmentação de legislações estaduais e municipais. 

### Impactos Práticos para Negócio e Tecnologia (Requisitos do Produto)

- Unificação de Cadastros e Regras: Fim da necessidade de manter parâmetros e tabelas de regras tributárias específicas para cada município ou estado. As regras de apuração e a base de cálculo passam a ser nacionais e uniformes.
- Tributação no Destino: A apuração da alíquota aplicável dependerá estritamente do local de consumo/entrega do bem ou serviço, tornando a validação de dados geográficos (CEP, Código IBGE) um elemento crítico nos cadastros e transações.
- Integração de Sistemas (APIs): O produto precisará conectar-se com os WebServices da Receita Federal (CBS) e com a Plataforma Nacional do Comitê Gestor do IBS para validação, emissão de guias e reconciliação financeira.
- Evolução de Layouts (DF-e): Adequação dos esquemas XML de Documentos Fiscais Eletrônicos (NF-e, NFC-e, NFS-e) para exibição e destaque individualizado da CBS e do IBS. 


## Princípios Constitucionais da Reforma Tributária do Consumo (RTC)

A sigla RTC significa Reforma Tributária do Consumo, esse material traz as diretrizes mestras que orientam a aplicação, fiscalização e criação do novo sistema tributário.

<img width="956" height="545" alt="image" src="https://github.com/user-attachments/assets/602745bf-7cc2-4478-bb6d-878432eaba63" />

Imagens Superiores (União x Estados/Municípios): Representam os dois ecossistemas do IVA Dual (CBS sob gestão da Receita Federal e IBS sob gestão do Comitê Gestor do IBS/COMSEFAZ/CNM/FNP), reforçando que estes princípios regem a atuação conjunta de todos esses entes públicos.

Princípios Constitucionais da Reforma Tributária (RTC)Previstos no Art. 145, § 3º da Constituição Federal, os princípios balizam a implementação técnica e operacional do novo IVA Dual (CBS + IBS):
   
- Simplicidade: Padronização nacional de normas, eliminando regimes fiscais conflitantes entre estados e municípios.
- Transparência: Exigência de visibilidade total da carga tributária destacada em cada transação.
- Justiça Tributária: Implementação de alíquotas reduzidas para itens essenciais e criação do sistema de Cashback (devolução de tributo a famílias elegíveis).
- Cooperação: Integração operacional e tecnológica entre a Receita Federal (CBS) e o Comitê Gestor do IBS (IBS).
- Defesa do Meio Ambiente: Aplicação do Imposto Seletivo (IS) sobre produtos/atividades que causem impacto ambiental ou à saúde.   


Requisitos de Negócio e Sistema (Visão de PM)

- Cálculo "Por Fora": Adequação da lógica matemática do motor de cálculo fiscal. O tributo deixa de incidir sobre a sua própria base de cálculo, tornando a precificação transparente e simplificada.
- Exibição Clara no Checkout e DF-e: Ajuste da UX/UI e dos leiautes de documentos fiscais para exibir a discriminação exata das alíquotas e valores de CBS, IBS e IS em cada item vendido.
- Parametrização do Imposto Seletivo (IS): Inclusão de flag/atributo no cadastro de produtos para identificar itens sujeitos à sobretaxa do IS.
- Elegibilidade a Cashback: Preparação do fluxo do checkout para captura e validação de CPF quando aplicável aos programas estaduais/federais de devolução de impostos.


## Visão Geral dos Princípios Constitucionais da RTC

Os cinco princípios constitucionais que orientam a Reforma Tributária do Consumo são:   
- Simplicidade : A unificação de tributos sobre o consumo em dois tributos principais — o Imposto sobre Bens e Serviços (IBS) e a Contribuição sobre Bens e Serviços (CBS) — reduz a complexidade do sistema atual, que envolve diversos tributos com regras distintas (ICMS, ISS, PIS, Cofins e IPI).
- Transparência: A reforma impõe que a alíquota total incidente sobre bens e serviços seja informada ao consumidor de forma destacada e obriga a disponibilização pública de dados fiscais, o que fortalece o controle social e facilita a compreensão sobre a carga tributária.
- Justiça Tributária: A justiça fiscal é buscada com a:
  - tributação no destino;
  - redução da cumulatividade; 
  - Alíquotas reduzidas para setores essenciais; e
  - mecanismos de devolução de tributos para famílias de baixa renda (cashback)
- Cooperação: Criação do Comitê Gestor do IBS, com representação de Estados, DF e Municípios, responsável pela administração do tributo, com normas uniformes e atuação integrada entre entes federativos.
- Defesa do meio ambiente: A reforma prevê a possibilidade de alíquotas específicas ou diferenciadas para produtos e serviços com impactos ambientais, bem como incentivos à sustentabilidade via instrumentos tributários.

Princípio 1: Simplicidade
- Conceito 
  - principal: Unificação de múltiplos impostos sobre o consumo em um modelo de IVA Dual.   
  - Impostos criados:IBS: Imposto sobre Bens e Serviços.
  - CBS: Contribuição sobre Bens e Serviços.
  - Impacto: Substitui o sistema anterior (que acumulava ICMS, ISS, PIS, Cofins e IPI), reduzindo a complexidade burocrática.
 
Princípio 2: Transparência
- Destaque ao consumidor: A alíquota total cobrada nos bens e serviços deve ser informada de forma clara e visível no momento da compra.
- Acesso aos dados: Exige a disponibilização pública dos dados fiscais.
- Objetivo: Garantir o controle social para que o cidadão entenda exatamente o valor dos impostos pagos.

## A Anatomicidade das Normas da Reforma Tributária: Da Constituição à Operação

<img width="735" height="412" alt="image" src="https://github.com/user-attachments/assets/c8266dda-d99f-4e34-ad71-f950c856fd56" />


1. Governação Dual (Os Órgãos Gestores)
   
- CGIBS e RFB: Representados pela figura com duas cabeças, simbolizando a atuação conjunta e harmonizada entre os dois órgãos de gestão do sistema IVA Dual:
  - RFB (Receita Federal do Brasil): Responsável pela administração do tributo de âmbito federal (CBS).
  - CGIBS (Comitê Gestor do IBS): Responsável pela gestão integrada dos entes subnacionais (Estados, Distrito Federal e Municípios).
 
2. Hierarquia e Granularidade Normativa (Analogia Anatómica)

A ordem descendente (da norma constitucional mais abrangente até à norma técnica mais específica) é explicada através dos componentes do sistema circulatório humano:

- EC 132 — Pulmão e Coração
  - Natureza: Emenda Constitucional nº 132/2023.
  - Papel: É o órgão vital e central do sistema; estabelece os princípios gerais e a estrutura base na Constituição
 
- LC 214 e LC 227 — Veias e Artérias Principais
  - Natureza: Leis Complementares de regulamentação.
  - Papel: Definem os grandes vasos e fluxos do imposto (regras gerais, alíquotas, não cumulatividade, isenções e regimes especiais)
 
- Regulamentos CBS/IBS (Decreto 12.955 e Resolução CGIBS 06) Veias e Artérias Médias
  - Natureza: Atos regulamentares do Poder Executivo e do Comitê Gestor.
  - Papel: Ramificam e detalham a aplicação das leis complementares para os diversos setores económicos.
 
- Notas Conjuntas IBS/CBS — Pequenos Vasos Capilares
  - Natureza: Orientações e especificações técnicas operacionais.
  - Papel: Chegam à extremidade do sistema (o contribuinte, o ponto de venda e os sistemas de emissão de nota fiscal/sistemas contabilísticos).
 
### Uniformidade entre IBS e CBS

Base Legal: Emenda Constitucional nº 132 | Artigo 149-B da Constituição Federal   Conceito-Chave: Princípio da Harmonização / Regra de Espelhamento do IVA Dual
 
  <img width="717" height="407" alt="image" src="https://github.com/user-attachments/assets/e890594a-a88a-4d07-b038-953de35d2a19" />

A regra constitucional do Artigo 149-B, que obriga o IBS (imposto subnacional de Estados e Municípios) e a CBS (contribuição federal) a adotarem exatamente as mesmas regras jurídicas e operacionais.   Embora a arrecadação seja dividida entre União, Estados e Municípios, para o contribuinte o sistema funciona com uma normatização unificada (modelo IVA Dual). 

2. Os 4 Pilares da Uniformização (Detalhamento)
Harmonia entre os dois tributos em quatro blocos principais:

Pilar 1: Elementos Fundamentais da Obrigação Tributária
As definições básicas de como o imposto nasce e quem o paga são idênticas:   
- Fatos Geradores: A atividade ou operação exata que faz surgir a obrigação de pagar o imposto.
- Bases de Cálculo: O valor sobre o qual a alíquota é aplicada.
- Hipóteses de Não Incidência: As situações operacionais em que a lei determina que não haverá cobrança.
- Sujeitos Passivos: A definição de quem é o responsável legal por recolher o tributo (empresas, prestadores de serviço, etc.).

Pilar 2: Imunidades
- Regra Única: As proteções constitucionais que proíbem a cobrança de tributos (como sobre livros, templos religiosos ou exportações) aplicam-se de forma idêntica e simultânea tanto ao IBS quanto à CBS.

Pilar 3: Regimes Diferenciados e Favorecidos
- Tratamento Setorial Uniforme: Caso um setor da economia (ex.: saúde, educação ou transporte urbano) tenha direito a alíquota reduzida ou regime especial, essa regra especial será exatamente a mesma nos dois impostos, sem divergências entre o governo federal e os governos locais.

Pilar 4: Não Cumulatividade e Creditamento
- Mecanismo do Crédito: A sistemática de abate do imposto pago nas etapas anteriores da cadeia (não cumulatividade) segue o mesmo conjunto de regras operacionais.
- Geração e Uso de Créditos: A forma como a empresa registra, comprova e utiliza seus créditos de IBS e CBS é idêntica.

**Por que isso é importante?Evita a burocracia do sistema antigo. Em vez de lidar com regras distintas para impostos federais (PIS/Cofins) e estaduais/municipais (ICMS/ISS), o contribuinte passa a calcular o IBS e a CBS sob uma única legislação harmonizada**

## Regras de Incidência e Alíquotas do IBS e CBS

<img width="717" height="407" alt="image" src="https://github.com/user-attachments/assets/f45a0d6f-508c-4364-8907-31eb7e051bf7" />

Base Legal: Emenda Constitucional nº 132 | Artigo 156-A da Constituição Federal   
Conceito-Chave: Regras Gerais de Funcionamento, Legislação Única e Autonomia das Alíquotas


8 pontos centrais do Artigo 156-A sobre o funcionamento do IBS e da CBS, alcance da tributação, o funcionamento das alíquotas nos entes federativos e a sistemática de apuração nacional.

1. Os 8 Blocos Operacionais (Detalhamento):

- Campo de Incidência Amplo
- Incidirão sobre operações com bens materiais ou imateriais, inclusive direitos, ou com serviços.
  - Significado: Abrange o consumo de forma ampla (mercadorias, bens digitais, licenças, direitos e prestação de serviços).
- Tributação da ImportaçãoIncidirão também sobre a importação.
  - Significado: Garante a neutralidade competitiva; bens e serviços vindos do exterior pagam o mesmo imposto que a produção nacional.
- Desoneração das Exportações
- Não incidirão sobre as exportações.   Significado: Mantém a competitividade das empresas brasileiras no mercado internacional (o tributo não é "exportado").   4. Legislação Única NacionalTerão legislação única e uniforme em todo o território nacional.   Significado: Elimina a guerra fiscal e a existência de milhares de leis municipais e estaduais diferentes.   5. Autonomia dos Entes (Alíquota Própria)Cada ente federativo fixará sua alíquota própria por lei específica.   Significado: Preserva a autonomia financeira de cada Estado, Distrito Federal e Município para definir a sua margem tributária.   6. Alíquota Uniforme no EnteA alíquota fixada pelo ente federativo será a mesma para todas as operações.   Significado: O ente fixa uma taxa padrão que se aplica a quase todos os produtos e serviços, evitando benefícios fiscais pontuais ou casuísticos.   7. Princípio do DestinoIBS será cobrado pelo somatório das alíquotas do Estado e do Município de destino da operação.   Significado: A arrecadação pertence ao local onde o bem ou serviço é efetivamente consumido, e não onde foi produzido.   8. Não Cumulatividade PlenaSerão não cumulativos, compensando-se o imposto devido pelo contribuinte com o montante cobrado sobre todas as operações nas quais seja adquirente.   Significado: Permite o abatimento integral de todos os tributos pagos na aquisição de insumos, bens e serviços ao longo da cadeia produtiva.   


## Fontes de Origem Procedente (Oficiais e Sem Risco de Inexactidão)

- Portal da Reforma Tributária – Ministério da Fazenda / Receita Federal:
      - Apresentações, Notas Técnicas e cronograma oficial do IVA Dual.
      - Acesso direto: gov.br/fazenda (Seção Reforma Tributária do Consumo).
- Portal Nacional da NF-e / ENCAT (Encontro Nacional dos Administradores Fiscais):
      - Especificações técnicas dos Documentos Fiscais Eletrônicos (Schemas XML, Notas Técnicas com novos campos do IBS/CBS).
      - Acesso direto: nfe.fazenda.gov.br / encat.org.br.
- Legislação Oficial (Portal do Planalto):
      - Emenda Constitucional nº 132/2023: Texto base constitucional.
      - PLP 68/2024: Projeto de Lei Complementar que institui e regulamenta a CBS, o IBS e o IS.
      - PLP 108/2024: Projeto de Lei Complementar do Comitê Gestor do IBS.

