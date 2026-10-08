<div align="center">

# 🇧🇷 Revisor de Português Brasileiro

### Escreva melhor, sem deixar de escrever como você.

Uma **Agent Skill** especializada em revisar, corrigir e aprimorar textos em português brasileiro, preservando a intenção, a personalidade e a voz de quem escreveu.

[![Idioma](https://img.shields.io/badge/Idioma-PT--BR-009739)](SKILL.md)
[![Padrão](https://img.shields.io/badge/Padr%C3%A3o-Agent%20Skills-2563eb)](https://agentskills.io/specification)
[![GitHub](https://img.shields.io/badge/GitHub-Enevinel-181717?logo=github)](https://github.com/Enevinel/revisor-portugues-brasileiro)

**[Conheça a skill](SKILL.md) · [Instalação](#instalação) · [Exemplos](#exemplos-de-uso) · [Contribuição](#contribuindo)**

</div>

---

## ✨ Sobre o projeto

O **Revisor de Português Brasileiro** foi criado para ir além da correção gramatical. Ele orienta agentes de IA a compreender **o que o autor quer dizer, para quem está escrevendo e como deseja se expressar** antes de modificar qualquer palavra.

> **Máxima qualidade, mínima distorção.** A melhor versão do texto que o autor quis escrever — não o texto que o revisor preferiria ter escrito.

### O que ele faz?

- **Corrige:** ortografia, acentuação, concordância, regência, crase, pontuação e sintaxe.
- **Aprimora:** clareza, coesão, coerência, fluidez, ritmo e estilo.
- **Preserva:** significado, fatos, grau de certeza, intenção, emoção e identidade do autor.
- **Adapta:** tom e nível de formalidade ao destinatário e ao contexto.
- **Protege:** datas, valores, nomes, identificadores, códigos, comandos e terminologia técnica.
- **Entrega:** textos naturais e prontos para copiar, sem justificativas desnecessárias.

## 🎯 O diferencial

Uma revisão ruim pode deixar um texto gramaticalmente correto e, ainda assim, **mudar o que a pessoa realmente queria dizer**.

Esta skill estabelece limites explícitos para evitar que o agente:

- Transforme **suspeitas em acusações** ou **possibilidades em certezas**.
- Crie promessas, sentimentos, compromissos ou fatos que não existiam.
- Converta uma conversa informal em uma mensagem artificialmente formal.
- Enfraqueça uma cobrança legítima ou intensifique um conflito sem solicitação.
- Altere dados, detalhes técnicos ou expressões juridicamente relevantes.
- Reescreva tudo quando uma pequena correção seria suficiente.

**O objetivo é preservar o autor — não substituí-lo.**

## 🧠 Modos de revisão

| Modo | Quando usar | O que esperar |
| --- | --- | --- |
| **Correção estrita** | “Corrija apenas a gramática.” | Alterações mínimas e pontuais. |
| **Revisão com polimento** | “Revise e melhore.” | Correção e fluidez com intervenção moderada. **É o padrão.** |
| **Reescrita aprimorada** | “Reescreva de forma mais elegante.” | Melhor estrutura, sem mudar a mensagem. |
| **Adaptação de tom** | “Deixe mais firme e respeitoso.” | Ajuste do estilo ao contexto e ao público. |
| **Revisão crítica** | “Aponte ambiguidades e possíveis interpretações.” | Texto revisado e observações relevantes. |

## 💬 Contextos atendidos

| Contexto | Cuidados principais |
| --- | --- |
| **Informal e conversacional** | Manter espontaneidade, regionalismos e oralidade adequada. |
| **Afetivo e emocional** | Preservar sentimentos sem melodrama ou promessas inventadas. |
| **Cobranças e conflitos** | Ser firme sem criar hostilidade ou acusações. |
| **Jurídico e administrativo** | Evitar alterações em fatos, condições e responsabilidades. |
| **Profissional e acadêmico** | Equilibrar objetividade, precisão e formalidade. |
| **Comercial e marketing** | Melhorar a comunicação sem inventar resultados ou garantias. |
| **Técnico e desenvolvimento** | Preservar comandos, APIs, logs, nomes e especificações. |

## 🔍 Antes e depois

**Exemplo 1 — Conversa informal**

**Original:**
> Oi, agente conversa amanhã pq hoje tô sem cabeça.

**Revisado:**
> Oi, a gente conversa amanhã porque hoje tô sem cabeça.

A correção mantém **“tô”** porque é natural nesse contexto.

**Exemplo 2 — Comunicação profissional**

**Original:**
> Segue os arquivos em anexo, preciso que vocês olha até sexta.

**Revisado:**
> Seguem os arquivos em anexo. Preciso que vocês deem uma olhada até sexta-feira.

**Exemplo 3 — Mensagem delicada**

**Original:**
> No domingo fui buscar minha filha no horário combinado mas você não respondeu minhas mensagens.

**Revisado:**
> No domingo, fui buscar minha filha no horário combinado, mas você não respondeu às minhas mensagens.

A revisão não cria alegações sobre motivos ou intenções da outra pessoa.

## 📦 Instalação

A skill usa o arquivo **[`SKILL.md`](SKILL.md)**, seguindo a estrutura do padrão [Agent Skills](https://agentskills.io/specification). Não precisa de dependências de execução: basta disponibilizar o arquivo ao agente compatível.

### OpenAI Codex — no projeto

Na raiz do projeto:

```bash
mkdir -p .agents/skills/revisor-portugues-brasileiro
curl -fsSL https://raw.githubusercontent.com/Enevinel/revisor-portugues-brasileiro/main/SKILL.md \
  -o .agents/skills/revisor-portugues-brasileiro/SKILL.md
```

### Claude Code — no projeto

```bash
mkdir -p .claude/skills/revisor-portugues-brasileiro
curl -fsSL https://raw.githubusercontent.com/Enevinel/revisor-portugues-brasileiro/main/SKILL.md \
  -o .claude/skills/revisor-portugues-brasileiro/SKILL.md
```

### Outros agentes

Copie `SKILL.md` para uma pasta chamada `revisor-portugues-brasileiro` no diretório de skills configurado para sua ferramenta. A descoberta e a ativação variam entre agentes: consulte a documentação do ambiente.

## 🚀 Exemplos de uso

Você pode invocar a skill com comandos naturais:

**Corrigir sem formalizar:**

```text
Corrija o português, mas mantenha meu jeito de falar:
[seu texto]
```

**Aprimorar a escrita:**

```text
Revise este texto e deixe-o mais claro, natural e elegante,
sem alterar o significado:
[seu texto]
```

**Ser firme sem ser agressivo:**

```text
Reescreva esta mensagem com firmeza e respeito.
Não invente fatos nem acrescente acusações:
[seu texto]
```

**Ajustar a emoção:**

```text
Deixe esta mensagem mais carinhosa e acolhedora,
sem criar sentimentos ou promessas que eu não expressei:
[seu texto]
```

**Revisar textos técnicos:**

```text
Melhore a clareza desta explicação técnica, mas não altere
comandos, endpoints, nomes de variáveis nem requisitos:
[seu texto]
```

**Identificar ambiguidades:**

```text
Revise esta mensagem e aponte ambiguidades relevantes,
sem transformar hipóteses em afirmações:
[seu texto]
```

## ⚙️ Como funciona

O comportamento da skill obedece a uma hierarquia editorial:

1. **Instrução explícita do usuário** — objetivo, público, tom e limites.
2. **Fidelidade aos fatos e ao significado** — nada de inventar, omitir ou intensificar.
3. **Voz e intenção** — manter a identidade e o posicionamento do autor.
4. **Correção linguística** — resolver erros e ambiguidades evitáveis.
5. **Naturalidade e elegância** — aprimorar quando houver ganho real.
6. **Concisão** — retirar o supérfluo sem perder conteúdo.

Antes da resposta, a skill orienta o agente a verificar coerência, gramática, tom, precisão, naturalidade e fidelidade.

## 📁 Estrutura

```text
revisor-portugues-brasileiro/
├── README.md    # Documentação e exemplos
└── SKILL.md     # Regras e instruções da skill
```

## ⚠️ Limitações

A skill é um conjunto de instruções para um modelo de linguagem; **não é um corretor determinístico nem garante ausência absoluta de erros**. Sua qualidade depende do agente utilizado e do contexto fornecido.

Em textos jurídicos ou de alto impacto, melhora a precisão **linguística**, mas não substitui a análise de um profissional habilitado nem garante que o documento esteja juridicamente livre de riscos.

## 🤝 Contribuindo

Contribuições são bem-vindas! Abra uma [issue](https://github.com/Enevinel/revisor-portugues-brasileiro/issues) com sugestões e exemplos reproduzíveis ou envie um [pull request](https://github.com/Enevinel/revisor-portugues-brasileiro/pulls).

Priorize melhorias que tornem a revisão mais **fiel, precisa, natural e útil**, sem comprometer a intenção original dos textos.

## 👤 Autor

**Lenivene Bezerra** — [Enevinel](https://github.com/Enevinel)

**Repositório:** https://github.com/Enevinel/revisor-portugues-brasileiro

---

<div align="center">

**Escrever melhor não significa deixar de escrever como você.**

Se o projeto for útil, considere deixar uma ⭐ no GitHub.

</div>
