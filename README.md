# tube_match  

Esse utilitário procura em um arquivo com dados de Tuberculose exportado do SINAN NET, registros cujos pacientes foram testados como positivo para HIV mas que não possuem notificação para AIDS na base de dados do SINAN NET.  
Para funcionar, basta que o usuário coloque os arquivos de exportação DBF de "Tuberculose" e "AIDS em adultos" na subpasta "base", rodar o utilitário e aguardar. Ao final do processamento, o arquivo "tube_aids.dbf" estará disponível na subpasta "out".

## Como usar?  

Faça o download do arquivo "tube_match.zip". Use sempre a versão mais atualizada que está disponível na seção "Releases";  

Descompacte o arquivo "tube_match.zip" usando o utilitário de descompactação de sua preferência;  

![x](/pictures/tube_match_pic1.jpg)  

A pasta resultante da descompactação deverá ficar no disco local C ou unidade local C;  

![x](/pictures/tube_match_pic2.jpg)  

Gere no SINAN NET os arquivos de exportação dos agravos de "AIDS adulto" e "Tuberculose" no módulo Ferramentas, item "Exportação (DBF)". Clique em "Exportar dados de identificação do paciente". Recomendamos que gere cada um desses arquivos por vez. Para Tuberculose, escolha uma data inicial e final nos campos "Período" e para "AIDS adulto", deixe os campos "Período" em branco, assim, o "tube_match" irá procurar os registros de casos de AIDS em toda a base de dados disponível, independente do ano em que foi notificado.  

![x](/pictures/tube_match_pic3.jpg)  

Os arquivos gerados estarão dentro da subpasta "BaseDBF" na pasta "SinanNet". Copie os arquivos "tubenet.dbf" e "aidsanet.dbf". Dependendo de como o Windows Explorer está configurado, esses dois arquivos também podem aparecer como "tubenet" e "aidsanet" sem as extensões ".dbf" junto. Se isso acontecer, não tem problema, pode copiá-los da mesma maneira.

![x](/pictures/tube_match_pic4.jpg)  

Uma vez copiados, os arquivos devem ser colados na subpasta "base", dentro da estrutura de subpastas do "tube_match".  

![x](/pictures/tube_match_pic5.jpg)  

Em seguida, rode o arquivo "tube_match.exe" que está no subdiretório "bin".  

![x](/pictures/tube_match_pic6.jpg)  

Aí é só aguardar o final do processamento.  

![x](/pictures/tube_match_pic7.jpg)  

Se o "tube_match.exe" encontrar alguma notificação de Tuberculose de paciente positivo para AIDS, que não esteja registrado nos casos de AIDS do SINAN NET, os dados do paciente estarão dispoíveis no arquivo "tube_aids.dbf" na subpasta "out" dentro da estrtura de diretórios do "tube_match".  

![x](/pictures/tube_match_pic8.jpg)  










