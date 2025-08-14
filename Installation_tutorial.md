## Tutorial de Instalação

### Instalando Dependências

Atualize o gerenciador de pacotes `apt` com o comando abaixo:

```bash
sudo apt-get update
sudo apt-get dist-upgrade -f
```

Verifique se tem o Python instalado, caso não esteja instale:

```Bash
python3 --version
sudo apt-get install python3 -f
```
Verifique se o módulo venv está instalado, caso não, instale:


```Bash
python3 -m venv --help
sudo apt-get install python3-venv -f
```

### Criação da venv e Instalação do Programa

Crie a venv "rankadmet" na pasta /opt/ e ative-a:

```Bash
sudo python3 -m venv /opt/rankadmet 
source /opt/rankadmet/bin/activate
```
Acesse o repositório no GitHub e copie o endereço do link da ultima versão do rankadmet (arquivo .whl). Use o comando abaixo fazer o download do arquivo:

```Bash
wget <link copiado>
```

Instale a ultima versão do rankadmet (arquivo .whl) e verfique a versão:

```Bash
sudo /opt/rankadmet/bin/pip install rankadmet* --force-reinstall
rankadmet --version
```

### Uso Diário

Ative o ambiente virtual do rankadmet e execute o programa.

```Bash
source /opt/rankadmet/bin/activate
```

Ao terminar, desative o ambiente virtual:

```Bash
deactivate
```

Atualizando
Para evitar conflitos, remova qualquer arquivo .whl existente no diretório atual:

```Bash
rm *.whl
```

Acesse o repositório no GitHub e copie o endereço do link da ultima versão do rankadmet (arquivo .whl). Use o comando abaixo fazer o download do arquivo:

```Bash
wget <link copiado>
```
Ative o ambiente virtual:

```Bash
source /opt/rankadmet/bin/activate
```
Instale o arquivo .whl da ultima versão do rankadmet:

```Bash
sudo /opt/rankadmet/bin/pip install rankadmet* --force-reinstall
```
Verifique a versão instalada:

```Bash
rankadmet --version
```
