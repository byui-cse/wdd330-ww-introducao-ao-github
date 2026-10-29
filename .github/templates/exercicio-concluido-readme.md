{% set socials_text -%}
{%- if exercise_title -%}
Acabei de concluir o exercício prático "{{ exercise_title }}" do GitHub Skills! 🎉
{%- else -%}
Acabei de concluir um exercício prático do GitHub Skills! 🎉
{%- endif %}

{{ repository_url }}

#GitHubSkills #OpenSource #GitHubLearn
{%- endset -%}

<div align="center">

# 🎉 Parabéns, {{ login }}! 🎉

<img src="https://octodex.github.com/images/welcometocat.png" height="200px" />

### 🌟 Você concluiu o exercício com sucesso! 🌟

## 🚀 Compartilhe a Sua Conquista!

**Mostre suas novas habilidades e inspire outras pessoas!**

<a href="https://twitter.com/intent/tweet?text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Compartilhar%20no%20X-1da1f2?style=for-the-badge&logo=x&logoColor=white" alt="Compartilhar no X" />
</a>
<a href="https://bsky.app/intent/compose?text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Compartilhar%20no%20Bluesky-0085ff?style=for-the-badge&logo=bluesky&logoColor=white" alt="Compartilhar no Bluesky" />
</a>
<a href="https://www.linkedin.com/feed/?shareActive=true&text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Compartilhar%20no%20LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Compartilhar no LinkedIn" />
</a>

### 🎯 E Agora?

**Continue aprendendo!**

[![](https://img.shields.io/badge/Voltar%20ao%20Exerc%C3%ADcio-%E2%86%92-1f883d?style=for-the-badge&logo=github&labelColor=197935)]({{ issue_url }})
[![GitHub Skills](https://img.shields.io/badge/Conhe%C3%A7a%20o%20GitHub%20Skills-000000?style=for-the-badge&logo=github&logoColor=white)](https://learn.github.com/skills)

*Não há maneira melhor de aprender do que criando coisas!* 🚀

</div>

---

Traduzido e adaptado pela BYU-Idaho a partir do [GitHub Skills](https://github.com/skills) &copy; GitHub, sob a [Licença MIT](https://gh.io/mit)
