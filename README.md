<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4f46e5,100:7c3aed&height=180&section=header&text=Victor%20Candido&fontSize=46&fontColor=ffffff&fontAlignY=36&desc=IA%20aplicada%20%C2%B7%20Seguran%C3%A7a%20de%20aplica%C3%A7%C3%B5es&descAlignY=58&descSize=18&animation=fadeIn" width="100%" alt="Victor Candido" />

<a href="https://estudeprumo.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=2800&pause=900&color=7C3AED&center=true&vCenter=true&width=620&lines=Fundador+e+CEO+da+Prumo;LLMs+em+produ%C3%A7%C3%A3o+com+usu%C3%A1rios+pagantes;Supabase%2C+RLS+e+chave+que+n%C3%A3o+vaza;Python+%C2%B7+TypeScript+%C2%B7+Next.js" alt="Digitando" />
</a>

</div>

Estudo Engenharia de Software em Brasília e fundei a Prumo com o Marcos Alan, uma plataforma de
estudos com IA para ENEM e concursos que está em produção, com usuários e pagamentos reais. Trabalho no
produto e no código, do front à infraestrutura, e boa parte do que faço gira em torno de colocar
modelos de linguagem em produção sem que eles virem um risco ou uma conta impagável.

## Em destaque: Prumo

<a href="https://github.com/burnoutscript/prumo">
  <img src="https://raw.githubusercontent.com/burnoutscript/prumo/main/docs/painel.png" width="100%" alt="Painel da Prumo" />
</a>

A Prumo gera simulados e trilhas a partir do objetivo do aluno, corrige redação com nota nas
cinco competências do ENEM e adapta o conteúdo ao cargo do concurso. Tem app web, iOS e Android
nativos, duelos entre alunos e um painel interno que mede custo, tokens e latência de cada
chamada de IA. O [estudo de caso](https://github.com/burnoutscript/prumo) conta a arquitetura e
as decisões de segurança. Os apps nativos, em SwiftUI e Jetpack Compose, têm um
[estudo de caso próprio](https://github.com/burnoutscript/prumo-apps).

## O que eu faço com IA

- Integro LLMs em fluxos que o usuário paga para usar: geração de questões, correção de redação
  com rubrica, tutoria e sugestão de temas.
- Meço custo e latência por requisição e escolho o modelo de cada plano com esses números.
- Uso agentes de código (Claude Code, Cursor, OpenCode) no dia a dia e rodo modelos abertos
  quantizados localmente, como o Qwen, para testar o que dá para fazer sem API paga.
- Trato texto de usuário como entrada não confiável. O [promptguard](https://github.com/burnoutscript/promptguard)
  saiu disso, com precisão e recall medidos num corpus separado.
- Protejo o que fica em volta do modelo: RLS no banco, chave privilegiada só no servidor e
  auditoria automática no CI.

## Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,nextjs,react,swift,kotlin&theme=dark" alt="Linguagens e frameworks" /><br/>
  <img src="https://skillicons.dev/icons?i=postgres,supabase,linux,cloudflare,githubactions,git&theme=dark" alt="Banco e infraestrutura" />
</p>

## Projetos

### Segurança de aplicações e IA

| Projeto | O que faz |
|---|---|
| [rls-guard](https://github.com/burnoutscript/rls-guard) | Audita as políticas de Row Level Security de um schema PostgreSQL/Supabase e sugere o SQL de correção |
| [supabase-hardening](https://github.com/burnoutscript/supabase-hardening) | Procura o que vaza num projeto Supabase além das tabelas: buckets públicos, funções expostas em `/rpc`, configuração de auth |
| [promptguard](https://github.com/burnoutscript/promptguard) | Detecta prompt injection antes do texto chegar ao LLM |
| [secret-scan](https://github.com/burnoutscript/secret-scan) | Acha chaves vazadas no código e no histórico do git, inclusive as que já foram apagadas |
| [loglens](https://github.com/burnoutscript/loglens) | Lê logs de nginx e sshd, aponta ataques e gera um resumo por IA sem mandar o log cru para fora |
| [headers-audit](https://github.com/burnoutscript/headers-audit) | Dá nota de A+ a F para os headers de segurança e os cookies de um site |

### Sistemas

| Projeto | O que faz |
|---|---|
| [minikv](https://github.com/burnoutscript/minikv) | Banco chave-valor persistente no estilo Bitcask, com recuperação de falha, compactação e servidor compatível com o protocolo do Redis |

Todos têm testes, CI rodando em Python 3.10 a 3.12 e um README que explica as decisões de
projeto.

<div align="center">

<img src="https://raw.githubusercontent.com/burnoutscript/burnoutscript/main/profile-3d-contrib/profile-night-rainbow.svg" width="100%" alt="Contribuições em 3D" />

[estudeprumo.com](https://estudeprumo.com)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,100:4f46e5&height=100&section=footer" width="100%" alt="" />

</div>
