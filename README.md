# BDbackupPostGree
Script com a funcionalidade de realizar o backup de um Banco de Dados PostGreSQL, com declaração de variáveis e regras de inicialização e realização do BackUo.

#SHELLSCRIPTBDbackupPostGree

#!/bin/sh

#bkp_estoque.sh

#DATA data no estilo dia-mes-ano.

DATA='/bin/date+%d-%m-%Y'

#NOME nome do arquivo de BackUP

#O Diretório onde o arquivo será salvo neste diretótio.

#/www/virtual/backup é uma pasta publica do apache.

#Em seguida o diretorio onde quiser guardar o BackUP.

NOME="/www/virtual/backup/estoque.sh-$DATA.sql"

#Variaveis PostGreSQL

HOST="localhost"

USER="bdpg"

PASSWORD="123456"

DATABASE="estoque.sh"

pg_dump -h $localhost -u $postgres -p $123456 $estoque.sh > $estoque.backup
