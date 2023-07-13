## 1. Implementação

Siga as etapas abaixo para implementar a Barra de Parceiros com exibição apenas com origem R7.COM

### Passo 1: Incluir o script no cabeçalho (head) do site

> 1. Abra o arquivo HTML do seu site<br>
> 2. Localize a seção <head> do documento<br>
> 3. Copie e cole o código abaixo no cabeçalho

```sh
<script async defer id="partners-bar" type="module" src="https://assets.r7.com/cda-partners-bar/cda-partners-bar/cda-partners-bar.esm.js"></script>
```
### Passo 2: Inserir os atributos no corpo <body> do seu site
    
> 1. Localize a seção <body> do documento<br>
> 2. Copie e cole o código abaixo e certifique-se de que seja o primeiro elemento logo após a abertura da tag
    
```sh
<cda-partners-bar style="height: 50px;display: block;" tag-manager="true" record-origin-only="true" no-follow='false'></cda-partners-bar>
```
---
## 2. Verificação

Após concluir a implementação, siga estas etapas para verificar se a Nova Barra de Parceiros está funcionando corretamente:

> 1. Abra seu site em um navegador<br>
> 2. Verifique se a Nova Barra de Parceiros é exibida corretamente na parte superior do site<br>
> 3. Teste a funcionalidade da barra, como cliques em links e interações
---
## 3. Sugestão Para Fixar a Barra
```sh
  .cda-container
    visibility: hidden;
    position: fixed;
    top: 0;
    left:0;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 50px;
```
---
## 4. Atributos

| Atributo                                | Descrição                                                                                   |
| --------------------------------------- | ------------------------------------------------------------------------------------------- |
| `record-origin-only`                    | Habilita a opção de exibir a barra somente quando o usuário acessar o site por meio do R7.  |
| `tag-manager`                           | Habilita o tagManager                                                                       |
| `no-follow`                             | Habilita o no-follow no menu                                                                |
| `style="height: 50px;display: block;"`  | Adiciona um espaço de 50px para a barra dessa forma impedindo erro de CLS                   |
