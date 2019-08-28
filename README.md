# GIT E GITHUB

Guia e revisão para iniciantes.

### Instalação

Instalar o GIT
https://git-scm.com/download

### SCENES - Objetivos

- [x] Criar pontos na história da produção do seu projeto
- [x] Verificar mudanças feitas no seu projeto

- [x] Começar um anova funcionalidade no seu projeto, mantendo o que já foi feito
- [x] Adicionar novas funcionalidades ao projeto em produção;
- [x] Deletar a branch da nova funcionalidade, depois de aplicar no projeto;

- [x] Colocar projeto na nuvem

## Começando Git no seu projeto

#### Iniciar linha do tempo do projeto: 

- `git init`
- Iniciado repositorio 
- Repositorio = Local onde ficam as alterações do projeto;

#### Criar uma nova página:
    
- comando: `touch nomearquivo.extensao`

#### Criar ponto na história do projeto

- 1# comando: `git add nomearquivo.extensao`
- 2# comando: `git add -m "mensagem para levar alteração"`

#### Verificar ponto criado na história do projeto

- comando: `git log`

#### Verificar status atual da aplicação

- comando: `git status`

## IMPORTANTE:
    - O arquivo alterado e não adicionado no repositório master do projeto aparecera como "untracked" no status do Git.
    - Apenas depois de adicionado (`git add nomearq.bla`) ele passa a ficar com status rastreado;

#### Verificar log de mudanças no arquivo 
    
- Git show no código do arquivo commitado;
- comando: `git show 'codigocommitado'`

#### Criar nova branch do projeto
    
- `git branch nomedabranch'`

#### Acessar branch
    
- `git checkout branch 'nomedabranch'`

#### Mesclar conteúdos de branchs distintas

- Estando na master ou branch que deseja inserir conteúdo 'alvo';
- `git merge 'nomedabranchalvo'`
- Alterações da branch alvo são inseridas na master ou branch em que foi rodada o comando git merge;

#### Deletar branch do projeto

- `git branch -D` // nomedabranch

#### Outros comandos

* `git status` // informa estado das alterações do nosso projeto
* `git show` // apresenta determinado ponto na historia, pode ser rodado junto com o código de commit da branch apos o '...show' 


### Comandos para criar repositorio remotos

* 1# Criar repositorio online no gitbhub, selecionar publico ou privado, criar readme.md e etc.
* `git remote add origin https://github.com/marioalvesx/nomedorepositoriocriadonogithub`

#### Visualizar repositorios remotos

* `git remote -v`

### Enviar repositorio local para repositorio online

* `git push nomebranch`
* Se é o primeiro 'push' do projeto, deve-se criar o repo. master remoto antes com o comando:
    * `git push -u origin master`

