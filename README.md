# Marketing-Bancario
Este é um script em Python que usa a biblioteca Streamlit para criar uma aplicação web para análise de dados de marketing bancário. A aplicação permite ao usuário carregar um arquivo de dados, filtrar os dados com base em várias opções de seleção e gerar gráficos que mostram informações sobre os dados filtrados.
# Importações

![import](https://user-images.githubusercontent.com/130613291/236697410-28eea8c8-d22a-4346-8eca-704a7e7a63da.png)

O script começa importando as bibliotecas necessárias, incluindo Pandas, Streamlit, Seaborn, Matplotlib e Pillow (para trabalhar com imagens). Em seguida, há algumas funções definidas, incluindo load_data, que lê um arquivo de dados (CSV ou XLSX), multiselect_filter, que filtra um DataFrame com base em várias opções de seleção, convert_df, que converte um DataFrame para um arquivo CSV e to_excel, que converte um DataFrame para um arquivo XLSX.


# Função principal da aplicação

Em seguida, há uma função principal chamada main. Dentro dessa função, a página da aplicação é configurada usando st.set_page_config, que define o título da página, o ícone da página e outras configurações.

Em seguida, a imagem é carregada usando Image.open e exibida na barra lateral da aplicação usando st.sidebar.image. Um botão é adicionado para permitir que o usuário carregue um arquivo de dados.

Se um arquivo de dados for carregado usando o file_uploader do Streamlit, os dados são lidos usando a função load_data e copiados para um novo DataFrame bank. Em seguida, os dados são exibidos usando st.write para mostrar as cinco primeiras linhas do DataFrame original.

O usuário pode usar uma série de opções de seleção na barra lateral para filtrar os dados. Essas opções incluem faixa etária, profissão, estado civil, default, financiamento imobiliário, empréstimo, meio de contato, mês do contato e dia da semana. Cada opção é implementada usando widgets do Streamlit, como st.slider, st.multiselect e st.radio.

Os dados são filtrados usando uma série de chamadas de método pipe, que são encadeadas para aplicar uma sequência de filtros ao DataFrame original. O resultado filtrado é armazenado no DataFrame bank.

Finalmente, os dados filtrados são usados para criar um gráfico usando Seaborn ou Matplotlib, dependendo da opção selecionada pelo usuário usando st.radio. O gráfico é exibido na página da aplicação usando st.pyplot. O usuário também pode baixar os dados filtrados como um arquivo CSV ou XLSX usando botões na barra lateral.



https://user-images.githubusercontent.com/130613291/236697468-2af4b242-b71d-4943-90fd-b29ebd8ce752.mp4

# Executando o Streamlit 
Essa função é um exemplo de como executar um aplicativo Streamlit no terminal do Windows. O Streamlit é uma biblioteca de código aberto usada para criar aplicativos da web interativos para análise de dados e visualização. A função começa mudando o diretório atual para onde o arquivo Python do aplicativo está localizado. Em seguida, é executado o comando streamlit run com o caminho do arquivo Python do aplicativo como argumento. O Streamlit inicia um servidor local e gera URLs de acesso à aplicação, uma para acesso local e outra para acesso pela rede. O usuário pode copiar a URL local e colá-la em um navegador para acessar o aplicativo.
# Streamlit funcionano


https://user-images.githubusercontent.com/130613291/236697522-35d04911-9d8d-47d6-8977-a08412005dc2.mp4

# Acessar o Streamlit Marketing-Bancario
[Clique aqui](http://localhost:8501/)
