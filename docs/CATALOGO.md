# Catálogo de frameworks — Cyber Frameworks

Inventário consolidado dos frameworks, padrões, bases de conhecimento e métodos já usados no portfólio (CyberFrameworks, Curupira/feeds) e das referências de telecom incorporadas em **13/11/2026**. A inclusão indica pertinência ao escopo, não endosso, certificação ou validação operacional. Confira versão, licença e condições na fonte original antes de reutilizar.

**Legenda de natureza:** `Framework` (estrutura de resultados ou processo) · `Base` (base de conhecimento/catálogo) · `Padrão` (especificação normativa ou esquema) · `Método` (técnica analítica) · `Guia` (orientação metodológica ou estudo).

## 1. Gestão de risco e desenvolvimento seguro

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [NIST CSF](https://www.nist.gov/cyberframework) | Framework | Que resultados de gestão de risco buscamos? | Não fornece regras de detecção nem técnicas de ataque |
| [NIST SSDF (SP 800-218)](https://csrc.nist.gov/projects/ssdf) | Framework | Que práticas incorporar ao ciclo de software? | Não certifica uma aplicação |

## 2. Comportamento adversário, defesa e resposta

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [MITRE ATT&CK](https://attack.mitre.org/) | Base | Que comportamento foi observado? | Mapeamento não comprova atribuição nem eficácia de controle |
| [MITRE D3FEND](https://d3fend.mitre.org/) | Base | Que contramedida técnica se relaciona ao comportamento? | Relação técnica ↔ defesa é semântica, não garantia de cobertura |
| [MITRE Engage](https://engage.mitre.org/) | Framework | Que objetivo defensivo guia o engajamento/deception? | Não é um produto de honeypot |
| [RE&CT](https://atc-project.github.io/atc-react/) | Base | Que ação de resposta a incidente aplicar em cada estágio? | Projeto comunitário; cobertura e atualização variáveis |
| [DeTT&CT](https://github.com/rabobank-cdc/dettect) | Framework | Qual é a nossa visibilidade e cobertura de detecção frente ao ATT&CK? | Pontuação é autoavaliada; depende da qualidade do inventário de fontes de dados |
| [CISA KEV](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) | Base | Esta CVE já tem exploração confirmada? | Ausência no catálogo não significa ausência de exploração |

## 3. Detecção e normalização de dados

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [Sigma / SigmaHQ](https://github.com/SigmaHQ/sigma) | Padrão | Como expressar a detecção de forma agnóstica ao SIEM? | Regras exigem tradução e ajuste ao ambiente (licença DRL 1.1) |
| [Elastic Common Schema (ECS)](https://www.elastic.co/guide/en/ecs/current/index.html) | Padrão | Como normalizar campos para consultas consistentes? | Esquema, não lógica de detecção; mapeamento por fonte é trabalho próprio |

| [UEBA — User and Entity Behavior Analytics (Palo Alto Cyberpedia)](https://www.paloaltonetworks.com.br/cyberpedia/what-is-user-entity-behavior-analytics-ueba) | Método | Que desvio de comportamento de usuário/entidade merece investigação? | Texto introdutório de fornecedor; linhas de base geram falsos positivos sem contexto |

## 4. Análise de inteligência e psicologia investigativa

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [ACH — Análise de Hipóteses Concorrentes (Heuer)](https://www.cia.gov/resources/csi/static/Pyschology-of-Intelligence-Analysis.pdf) | Método | Qual hipótese tem **menos** evidência inconsistente? | Reduz, não elimina, vieses (ancoragem, confirmação, automação) |
| PIR — Requisitos Prioritários de Inteligência | Método | Que decisão a inteligência precisa apoiar? | Conceito doutrinário; não há fonte normativa única — documentar a definição adotada |

## 5. Modelagem de ameaças (genérica)

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [MITRE CTID (Center for Threat-Informed Defense)](https://ctid.mitre.org/) | Base | Que projetos abertos de defesa informada por ameaças aplicar? | Portal de projetos; cada projeto tem escopo, versão e maturidade próprios |
| [MITRE CTID — Threat Modeling with ATT&CK](https://ctid.mitre.org/projects/threat-modeling-with-attack/) | Guia | Como integrar ATT&CK ao processo de modelagem de ameaças? | Orienta o processo; não substitui conhecimento do sistema modelado |
| [STRIDE / PASTA (visão OWASP)](https://owasp.org/www-community/Threat_Modeling_Process) | Método | Que classes de ameaça e que processo orientado a risco aplicar? | Categorias genéricas; precisam de adaptação ao domínio (ex.: telecom) |

## 6. Telecom e redes móveis (2G → 5G)

### Frameworks e catálogos de ameaças

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [MITRE FiGHT™ (5G Hierarchy of Threats)](https://fight.mitre.org/) | Base | Que táticas e técnicas adversárias são específicas de 5G? | Parte das técnicas é teórica/demonstrada em pesquisa, não observada em campo |
| [GSMA MoTIF (Mobile Threat Intelligence Framework)](https://www.gsma.com/get-involved/working-groups/content-type/article/establishing-motif-the-mobile-threat-intelligence-framework/) | Framework | Que TTPs reais aparecem em redes móveis e como compartilhá-las? | Detalhamento pode depender de acesso como membro da GSMA |
| [Bhadra Framework (arXiv 2005.05110)](https://arxiv.org/pdf/2005.05110) | Framework | Como estruturar o ciclo de vida de ataques em 2G/3G/4G? | Artigo acadêmico; não cobre 5G SA e não é mantido como base viva |
| [3GPP TR 33.926 (SCAS)](https://www.3gpp.org/dynareport/33926.htm) | Padrão | Quais ameaças e ativos críticos por função de rede 3GPP? | Garantia de segurança de equipamento; não é modelo de operação/detecção |

### Metodologia, estudos e órgãos reguladores

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [P1 Security — Threat Modeling in Telecom](https://www.p1sec.com/blog/threat-modeling-in-telecom-how-to-stop-designing-networks-that-beg-to-be-hacked) | Guia | Como modelar ameaças em quatro camadas numa operadora? | Artigo de fornecedor; perspectiva comercial |
| [ENISA — Signalling Security in Telecom (SS7, Diameter, 5G)](https://www.enisa.europa.eu/publications/signalling-security-in-telecom-ss7-diameter-5g) | Guia | Quais riscos de sinalização e interconexão priorizar? | Visão regulatória europeia; registrar a data da publicação |
| BSI — 5G Risk Analysis Framework (PDF) | Guia | Como aplicar PASTA e STRIDE na avaliação de risco 5G? | **Link direto pendente:** localizar o PDF oficial em [bsi.bund.de](https://www.bsi.bund.de/) e registrar versão/data |

## 7. Métodos autorais do portfólio

| Recurso | Natureza | Pergunta útil | Limite |
|---|---|---|---|
| [TCEM — Cyber-Threat-Context-Modeling](https://github.com/Ridd1kulusC0d3r/Cyber-Threat-Context-Modeling) | Método | Como ligar contexto a decisões defensivas rastreáveis? | Não é norma externa nem certificação |

## Comunidade e eventos (não são frameworks)

| Recurso | Uso |
|---|---|
| [Google DevFest](https://developers.google.com/community/devfest?hl=pt-br) | Evento comunitário para apresentar e discutir trabalhos do portfólio; não é referência metodológica |

## Como usar este catálogo

1. Comece pela **pergunta útil**, não pelo nome do framework.
2. Registre a versão exata e a data de consulta na [ficha](../templates/ficha.md).
3. Ao relacionar dois recursos (ex.: FiGHT ↔ ATT&CK, ATT&CK ↔ D3FEND), indique justificativa, granularidade e lacunas — não são equivalências automáticas.

[Início](../README.md) · [Matriz](MATRIZ.md) · [Referências](REFERENCIAS.md)
