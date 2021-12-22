# CursoPHPcomposerAlura
Aprofundando os conhecimento em php composer
Primeiro commit
- Na pasta raiz de o comando "composer init"
- ele ira pedir algumas informações
- no packege type escolha o que vc ira fazer
    - neste caso digitamos "library"



# Entendendo Autoload
 - A auto loado tem um padrão
 - Tem um namespace principal que fica tudo dentro da pasta src
 - "namespace Mix/class"
 - Caso tenha um subnamespace sera uma pasta
  "namespace Mix/Helper/class" 
  - O mix representa tudo o que está na src e o Helper é uma pasta
  dentro da src
  - Para configurar o autloado é no arquivo composer.json
  - colocando essa linha
     "autoload": {
        "psr-4": {
            "Mixfire\\Buscador"
        }
    }
  - Aqui vamos usar o padrão psr-4, que é padrão que implementa o modelo
  explicado aqui
  - Depois use o comando composer dumpload
  - Classmap serve para definirmo outros diretórios ou arquivos que queremos configurar de alguma maneira diferente, fora da src
  - podemos tbm o comando "files":["functions.php"]
    - Este comando diz que este arquivo sempre vai ser incluindo quando
    chamarmos uma função dele.