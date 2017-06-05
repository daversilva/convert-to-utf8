# ConvertToUTF8

Script feito em Python para mudança do encoding para UTF-8. Utilizando o Notepad++ para abrir o arquivo, trocar o encoding para UTF-8, salvar e fechar o arquivo.

**Ferramentas utilizadas:**
* Notepad++ v6.8.1
* Python Script v1.0.6

**Instalação do Python Script. Plugins -> Plugin Manager -> Show Plugin Manager**

![Alt text](https://cloud.githubusercontent.com/assets/8262095/10605044/f5aac02e-76fe-11e5-8ae9-77c53928ec71.png "Plugin Manager")

**Available -> Python Script**

![Alt text](https://cloud.githubusercontent.com/assets/8262095/10605097/68828096-76ff-11e5-855e-2924c4557e2a.png "Python Script")

**Criação do script**

![Alt text](https://cloud.githubusercontent.com/assets/8262095/10605213/37365f3e-7700-11e5-8ae7-9784b296f146.png "New Script")

**Escolha um nome para o script**

![Alt text](https://cloud.githubusercontent.com/assets/8262095/10605215/37800b52-7700-11e5-9d98-a7a921d91189.png "convert.py")

**Script para conversão em UTF-8**
```python
import os
import sys
filePathSrc="C:\\ConvertUTF8"
for root, dirs, files in os.walk(filePathSrc):
    for fn in files:
      if fn[-5:] == '.java':
        notepad.open(root + "\\" + fn)
        console.write(root + "\\" + fn + "\r\n")
        notepad.runMenuCommand("Encoding", "Convert to UTF-8")
        notepad.save()
        notepad.close()
```

**Depois é só executar o script. Python Script -> Scripts -> NOME_DO_SCRIPT.py**

![Alt text](https://cloud.githubusercontent.com/assets/8262095/10605214/374525be-7700-11e5-8553-70d0b320c142.png "convert.py")

Caso a execução do script não funcione pelo Notepad++, é bem provável que a versão do Python Script está corrompida, caso isso ocorra é só fazer a instalação do plugin manualmente.
