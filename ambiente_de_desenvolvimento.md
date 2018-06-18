# Ambiente de desenvolvimento

## Instalando programas necessarios
Para criar uma pagina HTML o processo é muito simples, todo computador que possui um browser ja tem tudo que é necessario para rodar uma pagina, então tudo que resta fazer é instalar um bom editor de texto.

Instalar o editor de texto sublime é muito simples, apenas acesse o [site do sublime](https://www.sublimetext.com/) baixe e instale ele. Caso você não goste do sublime existe outros editores de textos bem famosos como o [Atom](https://atom.io/) e o [Visual Studio](https://www.visualstudio.com/?rr=https%3A%2F%2Fwww.google.com%2F).

Apesar de não ser necessário a utilização do GIT para criar uma pagina web, ele facilita muito na hora de trabalhar em grupo, segue aqui como instalar o git:

Windowns:
Acesse o [site](https://gitforwindows.org/), faça o download do git e execute o programa de instalação.

Linux:
Digite os comandos no seu terminal:
```
$ apt-get install libcurl4-gnutls-dev libexpat1-dev gettext \ libz-dev libssl-dev
$ apt-get install git
```

Mac:
A forma mais facil de instalar o GIT no mac é por meio do instalador gráfico da [sourceforge](http://sourceforge.net/projects/git-osx-installer/)

---

## Criando pastas e arquivos .html e .css
De inicio, uma observação, se você está usando o linux e vc criar um arquivo e renomea-lo com a extenção .html ele ira funcionar perfeitamente, mas para o windowns isso não da tão certo. No windows se você renomear um arquivo para o nome "arquivo.html" ele mudou o nome mas não a extenção do arquivo, olhando as propriedades vemos algo como "arquivo.html.txt". Logo a forma mais facil de se criar um arquivo html no windows seria acessando o sublime, novo arquivo e colocar o nome .html.

Montando a estrutura da pasta(esse é apenas um exemplo, sintasse livre para montar sua estrutura de pasta da maneira que se sentir mais confortavel):
- Crie a pasta do projeto
- Dentro da pasta do projeto crie mais três pastas, chamadas html, css e imgs
- Abra a pasta do projeto pelo sublime
- Crie um arquivo.html dentro da pasta html com o nome que preferir, ex: "index.html"
- Faça o mesmo para o CSS
- Caso tenha alguma imagem que vá utilizar no projeto, coloque na pasta imgs

---

## Estrutura do arquivo html
O sublime possui diversos atalho que pode ajudar bastante. Dependendo da versão do sublime ao digitar html(ou !) seguito pela tecla tab ele já monta toda estrutura basica do html para você.

Estrutura basica:
```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Titulo</title>
</head>
<body>
	
</body>
</html>
```

---

## Importando arquivo CSS
Para importar um arquivo css basta so colocar a tag link no head do html, por exemplo:
```html
<link rel="stylesheet" type="text/css" href="mystyle.css">
```
O href representa o caminho para do arquivo html para o css, no caso da arquitetura de pastas que fizemos nos teriamos que voltar uma pagina para acessar a raiz do nosso projeto e a partir dela entrar na pasta css
```html
<link rel="stylesheet" type="text/css" href="../css/mystyle.css">
```

