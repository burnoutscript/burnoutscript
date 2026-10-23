### Victor Candido

Estudo Engenharia de Software em Brasília e sou cofundador da [Prumo](https://estudeprumo.com),
uma plataforma de estudos com IA para ENEM e concursos que está em produção com usuários
pagantes.

Meu foco é IA e segurança da informação. Na Prumo cuido do produto e do desenvolvimento, e boa
parte do trabalho de segurança passou por mim: RLS em todas as tabelas do Supabase, chave
`service_role` só no servidor, VPS atrás da Cloudflare e custo de IA medido por requisição. A
maior parte dos projetos abaixo saiu desse trabalho.

#### Segurança

| Projeto | O que faz |
|---|---|
| [rls-guard](https://github.com/burnoutscript/rls-guard) | Audita as políticas de Row Level Security de um schema PostgreSQL/Supabase e sugere o SQL de correção |
| [supabase-hardening](https://github.com/burnoutscript/supabase-hardening) | Procura o que vaza num projeto Supabase além das tabelas: buckets públicos, funções expostas em `/rpc`, configuração de auth |
| [secret-scan](https://github.com/burnoutscript/secret-scan) | Acha chaves vazadas no código e no histórico do git, inclusive as que já foram apagadas |
| [promptguard](https://github.com/burnoutscript/promptguard) | Detecta prompt injection antes do texto chegar ao LLM, com precisão e recall medidos num corpus próprio |
| [loglens](https://github.com/burnoutscript/loglens) | Lê logs de nginx e sshd, aponta ataques e gera um resumo por IA sem mandar o log cru para fora |
| [headers-audit](https://github.com/burnoutscript/headers-audit) | Dá nota de A+ a F para os headers de segurança e os cookies de um site |

#### Outros

| Projeto | O que faz |
|---|---|
| [minikv](https://github.com/burnoutscript/minikv) | Banco chave-valor persistente no estilo Bitcask, com recuperação de falha, compactação e servidor compatível com o protocolo do Redis |
| [prumo](https://github.com/burnoutscript/prumo) | Estudo de caso da arquitetura e das decisões de segurança da Prumo |

#### Stack

Python, TypeScript e Next.js, PostgreSQL e Supabase (RLS, Auth), Linux e hardening de VPS,
Cloudflare, APIs de LLM, GitHub Actions.

#### Contato

[estudeprumo.com](https://estudeprumo.com)
