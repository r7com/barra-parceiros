Siga as etapas abaixo para implementar a Nova Barra de Parceiros com exibição apenas com origem R7.COM

==========================================================================================================================================================

1. Implementação

  Passo 1: Incluir o script no cabeçalho (head) do site

    ●	Abra o arquivo HTML do seu site;
    ●	Localize a seção <head> do documento;
    ●	Copie e cole o seguinte código no cabeçalho:

        <script async defer id="partners-bar" type="module" src="https://assets.r7.com/cda-partners-bar/cda-partners-bar/cda-partners-bar.esm.js"></script>

  Passo 2: Inserir a tag HTML no corpo (body) do site
    ●	Localize a seção <body> do documento;
    ●	Copie e cole o seguinte código e certifique-se de que o código a seguir seja o primeiro elemento logo após a abertura do <body>:

        <cda-partners-bar tag-manager="true" record-origin-only="true" no-follow='false'></cda-partners-bar>

==========================================================================================================================================================

2. Verificação

Após concluir a implementação, siga estas etapas para verificar se a Nova Barra de Parceiros está funcionando corretamente:

  ●	Abra seu site em um navegador;
  ●	Verifique se a Nova Barra de Parceiros é exibida corretamente na parte superior do site;
  ●	Teste a funcionalidade da barra, como cliques em links e interações.

==========================================================================================================================================================

3. Sugestão Para Definir Altura

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

==========================================================================================================================================================

4. Atributos
-------------------------------------------------------------------------------------------------------------------
| Atributo           | Descrição                                                                                  |
|	record-origin-only | Habilita a opção de exibir a barra somente quando o usuário acessar o site por meio do R7. |
|	tag-manager        | Habilita o tagManager                                                                      |
|	no-follow          | Habilita o no-follow no menu                                                               |
-------------------------------------------------------------------------------------------------------------------

