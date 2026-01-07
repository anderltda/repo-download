# repo-download

#Na maquina crie ZIP único execute:
zip -r backup.zip eclipse

#Dividir em partes de 90 MB execute:
split -b 90m backup.zip backup.zip.part-

#Vai gerar:
backup.zip.part-aa 
backup.zip.part-ab 
backup.zip.part-ac

#Juntar e descompactar execute:
cat backup.zip.part-* > backup.zip unzip backup.zip