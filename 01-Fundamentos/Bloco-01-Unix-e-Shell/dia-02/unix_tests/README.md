01- Navegue até a pasta unix_tests;

cd ~/trybe/trybe-exercises/01-Fundamentos/Bloco-01-Unix-e-Shell/dia-02/unix_tests$ 

02- Crie um arquivo texto pelo terminal com o nome skills2.txt e adicione os valores Internet, Unix e Bash, um em cada linha.

cat > skills2.txt
Internet
Unix
Bash

ATALHO: ctrl+D para encerrar

03- Adicione mais 5 itens à sua lista de skills e depois imprima a lista ordenada no terminal. 🤓

cat >> skills2.txt 
add item 01 
add item 02
add item 03
add item 04
add item 05

ATALHO: ctrl+D para encerrar

04- Conte quantas linhas tem o arquivo skills2.txt.

wc -l skills2.txt

05- Crie um arquivo chamado top_skills.txt usando o skills2.txt, contendo as 3 primeiras skills em ordem alfabética.

sort skills.txt | head -3 | cat > top_skills.txt


06- Crie um novo arquivo chamado phrases2.txt pelo terminal e adicione algumas frases de sua escolha.
 
cat > phrases2.txt

adicionei uma musica

07- Conte o número de linhas que contêm as letras br.

grep br phrases2.txt | wc -l

08- Conte o número de linhas que não contêm as letras br.

grep -v br phrases2.txt | wc -l

09- Adicione dois nomes de países ao final do arquivo phrases2.txt.

cat >> phrases2.txt 
Canadá
Chile 

ATALHO ctrl+ D

10- Crie um novo arquivo chamado bunch_of_things.txt com os conteúdos dos arquivos phrases2.txt e countries.txt

cat phrases2.txt ~/trybe/trybe-exercises/01-Fundamentos/Bloco-01-Unix-e-Shell/dia-01/
unix_tests/countries.txt > bunch_of_things.txt

11- Ordene o arquivo bunch_of_things.txt.

sort bunch_of_things.txt -o bunch_of_things.txt
