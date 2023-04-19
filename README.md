# Utilizando-Plugins-no-Webpack

. Para utilizar um plugin no webpack precisamos primeiro instalar o pacote do plugin como dependência de desenvolvimento.

. Estamos utilizando o plugin  “mini-css-extract-plugin”.
Que é um plugin para extrair o CSS incluindo no ponto de entrada em um arquivo separado do nosso arquivo javascript. Comece instalando o plugin:

# npm install --save-dev mini-css-extract-plugin

. Agora que já instalamos o plugin, precisamos ajustar as configurações do webpack para incluir o plugin e utilizá-lo nos arquivos CSS:

. Repare que para esse plugin isso ocorre em duas etapas, primeiro incluímos a instância da classe MiniCssExtractPlugin no array “plugins”, e então substituímos o “style-loader” pelo loader do plugin (porque agora não iremos carregar estilos com o javascript e sim incluir estilos em um css separado)

. Por fim, só precisamos ajustar o arquivo index.html para incluir o novo arquivo css que geramos
