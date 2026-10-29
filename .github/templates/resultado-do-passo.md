{%- set all_passed = (results_table | selectattr("passed") | length) == (results_table | length) %}

{%- if all_passed %}

## Passo {{ step_number }} - Aprovado ✅

{%- else %}

## Passo {{ step_number }} - Reprovado ❌

{%- endif %}

{%- if all_passed %}
<img src="https://octodex.github.com/images/inflatocat.png" align="right" height="150px" alt="Imagem indicando que o passo foi aprovado" />
{%- else %}

<img src="https://octodex.github.com/images/spidertocat.png" align="right" height="100px" alt="Imagem indicando que o passo foi reprovado" />
Algumas verificações falharam. Confira os resultados abaixo e tente de novo.

Hora de encontrar o erro! 🤔
{%- endif %}

| Situação | Descrição |
| ------ | ----------- |

{%- for row in results_table %}
| {% if row.passed -%}✅ - Aprovado{%- else -%}❌ - Reprovado{%- endif %} | {{ row.description }} |
{%- endfor %}
