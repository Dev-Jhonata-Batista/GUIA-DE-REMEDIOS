# Guia Rápido de Remédios

Site informativo sobre remédios de farmácia que podem ser comprados sem receita,
feito para a atividade da Unidade 2 da disciplina Desenvolvimento Front-end para Web (UNIPÊ).

A ideia é ajudar quem está com um sintoma simples, como enjoo ou dor de cabeça, e não
sabe qual remédio pode tomar. Cada página mostra uma resposta rápida, uma tabela com os
remédios sem receita, os cuidados e quando é hora de procurar um médico.

> Este site é só informativo e não substitui a orientação de um médico ou farmacêutico.

## Páginas

O site tem 6 páginas, todas dentro da pasta `html/`:

| Arquivo | Conteúdo |
|---|---|
| `html/index.html` | Página inicial com os sintomas, as tarjas dos remédios, cuidados gerais e telefones úteis |
| `html/enjoo.html` | Enjoo e vômito |
| `html/dor-e-febre.html` | Dor de cabeça e febre (com o alerta sobre dengue) |
| `html/azia-gases-colica.html` | Azia, gases e cólica |
| `html/diarreia.html` | Diarreia e hidratação |
| `html/alergia.html` | Alergia |

Todas as páginas têm o mesmo menu lateral, então dá para ir de qualquer página para qualquer outra.

## Organização das pastas

```
guia-remedios/
├── html/          páginas do site (cada uma com o seu CSS)
├── img/           ícones em SVG
└── README.md
```

O CSS de cada página fica dentro da própria página, na tag `<style>` do `<head>`.
Como as páginas ficam dentro de `html/`, elas usam `../` para chegar nas imagens
(exemplo: `<img src="../img/enjoo.svg">`).

## Estrutura das páginas

Todas as páginas usam o mesmo layout com `div`, como foi visto em aula:

```
div#site
├── div#header      título do site
├── div#conteudo
│   ├── div#menu    menu lateral (float: left)
│   └── div#main    conteúdo da página
└── div#footer      rodapé
```

## O que pratiquei

- Layout com `div` e `id` (header, menu, main e footer)
- CSS interno, com a tag `<style>` dentro do `<head>` de cada página
- Atributo `style` direto na tag (CSS inline) nos títulos e destaques de cada página
- Cores em RGB (`rgb(30, 111, 92)`) e em hexadecimal
- Seletores de tag, de id (`#menu`), de classe (`.alerta`) e de descendente (`#menu a`)
- Box model: `margin`, `padding` e `border`
- `float` e `clear` para montar as colunas
- `:hover` e a classe `ativo` para marcar no menu a página que está aberta
- `display: block` e `inline-block`
- Tabelas, listas e imagens
- Caminhos relativos entre pastas (`../`)
- `meta viewport` e um ajuste simples para celular com `@media`

## De onde vieram as informações

- Lista de Medicamentos Isentos de Prescrição da Anvisa (IN nº 285/2024, atualizada pela IN nº 404/2025)
- Bulas dos medicamentos citados
- Orientações do Ministério da Saúde sobre remédios na suspeita de dengue

## Como abrir

1. Clone o repositório (ou baixe o arquivo .zip pelo botão "Code" do GitHub):
```bash
git clone https://github.com/Dev-Jhonata-Batista/guia-remedios.git
```
2. Entre na pasta do projeto.
3. Abra o arquivo `html/index.html` no navegador (dois cliques no arquivo já funcionam).

Não é preciso instalar nada.

## Tecnologias

- HTML5
- CSS3

## Autor

Feito por **Jhonata Batista**, estudante de Ciência da Computação.

- GitHub: [Dev-Jhonata-Batista](https://github.com/Dev-Jhonata-Batista)
- LinkedIn: [linkedin.com/in/dev-jhon](https://www.linkedin.com/in/dev-jhon)
