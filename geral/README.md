## 1. Implementação

Siga as etapas abaixo para implementar a Barra de Parceiros

### Passo 1: Incluir o script no cabeçalho (head) do site

> 1. Abra o arquivo HTML do seu site<br>
> 2. Localize a seção <head> do documento<br>
> 3. Copie e cole o código abaixo no cabeçalho

```sh
<script id="partners-bar" type="module" src="https://assets.r7.com/cda-partners-bar/cda-partners-bar/cda-partners-bar.esm.js"></script>
```

A tag script deverá apenas ter o type="module", sem necessidade de async e defer. Por padrão o type module já se comporta sem bloquear a renderização da página e implicitamente já existe um modo "defer" quando usa type module, e portato, o script pode ficar no <head> do HTML. É importante retirar os scripts lazy load, cache entre outros plugins dentro da barra para evitar problemas de performance pois o próprio browser vai cachear o script após a primeira request.

---

### Passo 2: Inserir os atributos no corpo <body> do seu site
    
> 1. Localize a seção <body> do documento<br>
> 2. Copie e cole o código abaixo e certifique-se de que seja o primeiro elemento logo após a abertura da tag
    
```sh
<cda-partners-bar tag-manager="true" record-origin-only="false" no-follow='true'></cda-partners-bar>
```
---
## 2. Verificação

Após concluir a implementação, siga estas etapas para verificar se a Nova Barra de Parceiros está funcionando corretamente:

> 1. Abra seu site em um navegador<br>
> 2. Verifique se a Nova Barra de Parceiros é exibida corretamente na parte superior do site<br>
> 3. Teste a funcionalidade da barra, como cliques em links e interações
---

## 3. Atributos

| Atributo                                | Descrição                                                                                                   |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `record-origin-only`                    | Habilita a opção de exibir a barra somente quando o usuário acessar o site por meio do R7 com true ou false |
| `tag-manager`                           | Habilita o tagManager                                                                                       |
| `no-follow`                             | Habilita ou Desabilita o no-follow para os itens de menu                                                    |

