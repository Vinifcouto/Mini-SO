# Mini-SO

Objetivo do SO: 
  - Criar um sistema de desenhos através de comandos interativos parecidos com a IDE "SuperLogo".
  - Não será desenvolvido um sistema completo de arquivos, apenas um sistema onde é possível salvar, editar ou excluir arquivos.
  - Não será desenvolvido drivers, pois serão utilizados os recursos diretamente da BIOS na arquitetura de 16 bits.
  - O sistema será desenvolvido de forma didática para pessoas que querem entender como funciona um sistema operacional simples e para crianças começarem a interagir com este mundo.

Ferramentas utilizadas:
  - O sistema será executado em um pendrive ou diskette, rodando em máquina real ou virtual.
  - Serão utilizados o Nasm para manipulações em Assembly, o Fergo Raw para criação de arquivos de imagem e Rufus 3.9.
  - Link do Nasm: https://www.nasm.us/pub/nasm/releasebuilds/2.14.03rc2/win64/
  - Link do Fergo Raw: https://www.fergonez.net/softwares/fraw
  - Link do Rufus: https://rufus.ie/downloads/
  - Será utilizado também um editor chamado Notepad++

Desenvolvimento:
  - Primeiramente fazemos o download do Nasm, do Fergo Raw e do Rufus 3.9. Em seguida, efetuamos a instalção do Nasm, inicializamos o Rufus 3.9 e extraimos o Zip do Fergo Raw. Entretanto, já encontramos um problema tentando abrir o arquivo extraído do Zip em questão. Aparece uma mensagem alegando que o componente "MSCOMCTL.OCX" ou uma de suas dependências não está corretamente registrada: um arquivo está faltando ou é inválido. Foi sugerido o uso de uma máquina virtual, porém os respectivos autores deste repositório não conseguiram solucionar ainda este problema. Evidentemente, será buscado uma solução futura para este problema.
  - Após a solução deste problema, deve-se configurar as variáveis de ambiente. Onde pegamos primeiramente o diretório do Nasm, abrimos as propriedades do computador e procuramos variáveis de ambiento no buscador e selecionamos o mesmo, posteriormente selecionamos a variável de sistema chamada de "path" e colamos o diretório do Nasm no campo chamado de "Valor da variável:" seguido de um clique no botão "ok". Após essa operação, feche as abas e abra o CMD e digite "nasm version" e será possível visualizar que agora o Nasm é uma variável de ambiente e poderá ser executada em qualquer lugar do computador.
  - Em seguida devemos organizar os arquivos do nosso SO, onde criamos uma pasta chamada "OSFiles" contendo outras duas pastas chamadas de "FergoRaw" e "Rufus", pasta essas que deverão conter as suas respectivas ferramentas detalhadas anteriormente.
  - Após isso, abrimos o editor Notepad++ para criar o BAT, onde executamos as instruções realizadas no vídeo. Por fim, no final do segundo vídeo o autor ensina como montar arquivos .ASM pelo Nasm.
  - No terceiro vídeo, é ensinado como baixar e instalar o Rufus 2.18 e máquina virtual da Oracle. O autor em seguida, mostra a execução e configuração do VirtualBox, a criação de uma máquina virtual e confuguração do USB. Por fim, o apresentador do vídeo demonstra como visualizar o número do pendrive pelo Windows e como gerar o arquivo .vmdk que conecta no USB. E por última instância, o autor revisa as configurações do VirtualBox.

Autores:
  -Emilaine Prado Correia Fagundes e Vinicius Ferreira Couto.
