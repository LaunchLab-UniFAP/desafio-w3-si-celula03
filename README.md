## Propriedade Intelectual e Governanca de Configuracao

### 1. Licenciamento Open-Source (Apache License 2.0)
Para o ecossistema de monitorizacao de endemias urbanas gerido pelo consorcio internacional, foi adotada a licenca Apache 2.0.
* **Concessao Expressa de Patentes**: Diferente de licencas permissivas simples como MIT ou BSD, a Apache 2.0 protege os membros contra litigios futuros (Seccao 3), garantindo que contribuicoes algoritmicas de predicao de vetores nao sejam bloqueadas por patentes posteriores de instituicoes participantes.
* **Preservacao de Direitos e Atribuicao**: Exige a manutencao explicita das notas de direitos de autor e dos avisos legais originais em qualquer distribuicao ou bifurcacao (fork), salvaguardando a autoria coletiva da celula e das entidades de saude publica envolvidas.
* **Viabilidade Comercial e Colaborativa**: Permite que paises membros adaptem o codigo as suas realidades locais sem impor clausulas virais (como as da GPL), facilitando parcerias publico-privadas na contencao de surtos.

### 2. Conformidade Legal e Auditoria Internacional
* **Compliance Multi-Jurisdicional**: O projeto opera sob as diretrizes da LGPD (Brasil), GDPR (Uniao Europeia) e HIPAA (EUA), formalizadas no manifesto docs/governanca_dados.json.
* **Anonimizacao Mandatoria de Pacientes**: Proibe-se a inclusao de dados clinicos nominais diretos. As metricas de dispersao espacial utilizam agregacao por raio minimo (k-anonimato) e pseudonimizacao criptografica para impedir a reidentificacao de pacientes.
* **Rastreabilidade e Isonomia**: Nenhuma modificacao e aceite na branch principal sem revisao previa. Todos os commits sao submetidos a validacao semantica (Conventional Commits) e auditados periodicamente atraves do script scripts/auditar_commits.py, gerando relatorios com os hashes assinados e metricas de distribuicao de esforco dos membros da celula.