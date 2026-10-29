# image-sources

The screenshots in `.github/images/` come from the original English exercise
([skills/introduction-to-github](https://github.com/skills/introduction-to-github), MIT License).
The GitHub UI stays in English (students see it that way). Only the text the student types was changed so it
matches the translated instructions:

| Original | Portuguese |
| --- | --- |
| `my-first-branch` | `primeiro-branch` |
| `PROFILE.md` | `PERFIL.md` |
| `Add PROFILE.md` | `Adicionar PERFIL.md` |
| `Welcome to my GitHub profile!` | `Bem-vindo(a) ao meu perfil do GitHub!` |
| `Add my first file` | `Adicionar meu primeiro arquivo` |
| PR description | `Criei um novo branch, criei um arquivo e fiz um commit!` |
| Repository name `skills-introduction-to-github` / `intro-to-github` | `introducao-ao-github` (the name the "Copiar Exercício" button gives the copy) |
| `generated from skills/introduction-to-github` | `generated from byui-cse/wdd330-ww-introducao-ao-github` |
| Example profile README (`Hi there`, `I'm currently working on something cool!`, ...) | `Olá`, `Estou trabalhando em algo legal!`, `Estou aprendendo com a ajuda do`, `Pergunte-me sobre o GitHub` |

Images with only GitHub UI text (`create-new-file-option.png`, `merge-pull-request-button.png`) are unchanged.
The sample user's names (`octocat`, `octocato`) and bio in `example-profile-readme.png` were kept.

To regenerate (Windows, Python + Pillow), from the repository root:

    python image-sources/traduzir-prints.py <folder-with-original-images> .github/images

For another language, edit the new texts in `traduzir-prints.py` and keep the names consistent with the
step files (`.github/steps/`) and the workflows (`.github/workflows/`), which check the branch name, the file
name and the pull request title.
