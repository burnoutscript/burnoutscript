<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4f46e5,100:7c3aed&height=190&section=header&text=Victor%20Candido&fontSize=48&fontColor=ffffff&fontAlignY=36&desc=Fundador%20e%20CEO%20da%20Prumo%20%C2%B7%20IA%20aplicada%20%C2%B7%20Seguran%C3%A7a&descAlignY=58&descSize=17&animation=fadeIn" width="100%" alt="Victor Candido" />

<a href="https://estudeprumo.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=2800&pause=900&color=7C3AED&center=true&vCenter=true&width=640&lines=Fundador+e+CEO+da+Prumo;Web%2C+iOS+e+Android+em+produ%C3%A7%C3%A3o;LLMs+com+usu%C3%A1rios+pagantes;Supabase%2C+RLS+e+chave+que+n%C3%A3o+vaza" alt="Digitando" />
</a>

<a href="https://estudeprumo.com"><img src="https://img.shields.io/badge/estudeprumo.com-7c3aed?style=for-the-badge&logo=googlechrome&logoColor=white" alt="estudeprumo.com" /></a>
<a href="https://github.com/burnoutscript/prumo"><img src="https://img.shields.io/badge/estudo_de_caso-4f46e5?style=for-the-badge&logo=github&logoColor=white" alt="Estudo de caso" /></a>
<a href="https://github.com/burnoutscript/prumo-apps"><img src="https://img.shields.io/badge/apps_iOS_e_Android-312e81?style=for-the-badge&logo=apple&logoColor=white" alt="Apps iOS e Android" /></a>

</div>

Estudo Engenharia de Software em Brasília e fundei a Prumo com o Marcos Alan. É uma plataforma
de estudos com IA para ENEM e concursos, com site, app de iPhone e app de Android, em produção
com alunos e pagamentos reais. Trabalho no produto e no código, do banco à tela, e quase tudo
que faço gira em torno de colocar modelos de linguagem em produção sem que eles virem um risco
ou uma conta impagável.

## Prumo

<a href="https://github.com/burnoutscript/prumo">
  <img src="https://raw.githubusercontent.com/burnoutscript/prumo/main/docs/painel.png" width="100%" alt="Painel da Prumo na web" />
</a>

A Prumo monta simulados e trilhas a partir do objetivo do aluno, corrige redação com nota nas
cinco competências do ENEM e adapta o conteúdo ao cargo do concurso. Tem duelos entre alunos,
flashcards com revisão diária e um painel interno que mede custo, tokens e latência de cada
chamada de IA.

<a href="https://github.com/burnoutscript/prumo-apps">
  <img src="https://raw.githubusercontent.com/burnoutscript/prumo-apps/main/docs/capa.png" width="100%" alt="Apps nativos da Prumo para iOS e Android" />
</a>

Os apps são nativos: SwiftUI no iPhone e no iPad, Jetpack Compose no Android, com widgets,
Live Activity e treino guiado para o teste físico de concursos. Os três clientes usam o mesmo
banco e a mesma API, e nenhuma chave privilegiada vai dentro do app.

| | |
|---|---|
| [prumo](https://github.com/burnoutscript/prumo) | Estudo de caso da plataforma: arquitetura, custo de IA e decisões de segurança |
| [prumo-apps](https://github.com/burnoutscript/prumo-apps) | Estudo de caso dos apps iOS e Android: por que nativo, assinatura, animação dos exercícios |

## O que eu faço com IA

- Integro LLMs em fluxos que o usuário paga para usar: geração de questões, correção de redação
  com rubrica, tutoria e montagem de treino e dieta.
- Deixo a conta com o código e o texto com o modelo. Na Prumo, índice de edital e meta de
  calorias são calculados em código; a IA só recebe os números prontos.
- Meço custo e latência por requisição e escolho o modelo de cada plano com esses números.
- Uso agentes de código (Claude Code, Cursor, OpenCode) no dia a dia e rodo modelos abertos
  quantizados localmente, como o Qwen.
- Trato texto de usuário como entrada não confiável. O [promptguard](https://github.com/burnoutscript/promptguard)
  saiu disso, com precisão e recall medidos num corpus separado.
- O agente instala pacote sozinho o tempo todo. Na Prumo o lockfile tem 660 pacotes e eu escolhi
  uns 20. O [bouncer](https://github.com/burnoutscript/bouncer) analisa cada um antes de instalar.

## Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,nextjs,react,swift,kotlin&theme=dark" alt="Linguagens e frameworks" /><br/>
  <img src="https://skillicons.dev/icons?i=postgres,supabase,linux,cloudflare,githubactions,git&theme=dark" alt="Banco e infraestrutura" />
</p>

## Projetos open source

### Segurança de aplicações e IA

| Projeto | O que faz |
|---|---|
| [bouncer](https://github.com/burnoutscript/bouncer) | Analisa cada pacote que o agente de IA vai instalar (npm, PyPI, curl \| sh, servidores MCP, skills) e bloqueia malware antes de rodar. Também executa o pacote num sandbox com credenciais falsas para ver o que ele tenta enviar |
| [rls-guard](https://github.com/burnoutscript/rls-guard) | Audita as políticas de Row Level Security de um schema PostgreSQL/Supabase e sugere o SQL de correção |
| [supabase-hardening](https://github.com/burnoutscript/supabase-hardening) | Procura o que vaza num projeto Supabase além das tabelas: buckets públicos, funções expostas em `/rpc`, configuração de auth |
| [promptguard](https://github.com/burnoutscript/promptguard) | Detecta prompt injection antes do texto chegar ao LLM |
| [secret-scan](https://github.com/burnoutscript/secret-scan) | Acha chaves vazadas no código e no histórico do git, inclusive as que já foram apagadas |
| [loglens](https://github.com/burnoutscript/loglens) | Lê logs de nginx e sshd, aponta ataques e gera um resumo por IA sem mandar o log cru para fora |
| [headers-audit](https://github.com/burnoutscript/headers-audit) | Dá nota de A+ a F para os headers de segurança e os cookies de um site |

### Ferramentas para agentes de IA

| Projeto | O que faz |
|---|---|
| [skillcheck](https://github.com/burnoutscript/skillcheck) | Linter para skills do Claude Code, Cursor e Codex: dá nota de 0 a 100 e aponta gatilho fraco, colisão entre skills, link quebrado e custo em tokens |
| [sales-skills](https://github.com/burnoutscript/sales-skills) | 16 skills de vendas B2B para agentes: prospecção, discovery, demo, objeções, proposta, negociação e revisão de pipeline com MEDDPICC |

### Sistemas

| Projeto | O que faz |
|---|---|
| [minikv](https://github.com/burnoutscript/minikv) | Banco chave-valor persistente no estilo Bitcask, com recuperação de falha, compactação e servidor compatível com o protocolo do Redis |

Todos têm testes e CI (Python 3.10 a 3.12, ou Node 18 a 22 em Linux, macOS e Windows) e um
README que explica as decisões de projeto.

<div align="center">

<br/>

<img src="https://raw.githubusercontent.com/burnoutscript/burnoutscript/main/assets/contadores.svg" alt="Estrelas, contribuições e repositórios" />

<br/><br/>

<sub>visitas ao perfil</sub><br/>
<img src="https://count.getloli.com/@burnoutscript?name=burnoutscript&theme=cat-girls-yay&padding=6&offset=0&align=top&scale=1&pixelated=1&darkmode=0" alt="Visitas" />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,100:4f46e5&height=100&section=footer" width="100%" alt="" />

</div>
