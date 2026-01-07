# Na maquina crie ZIP único execute:
zip -r backup.zip eclipse

# Dividir em partes de 90 MB execute:
split -b 90m backup.zip backup.zip.part-

# Vai gerar 
backup.zip.part-aa <br>
backup.zip.part-ab <br>
backup.zip.part-ac <br>
backup.zip.part-ad <br>
backup.zip.part-a... <br>

# Juntar e descompactar execute:
cat backup.zip.part-* > backup.zip <br>
unzip backup.zip