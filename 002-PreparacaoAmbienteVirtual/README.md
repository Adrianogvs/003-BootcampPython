# Configurando Ambientes Virtuais com Pyenv


## Introdução ao Pyenv

O **Pyenv** é uma ferramenta que permite gerenciar múltiplas versões do Python em um único sistema. Com ele, é possível instalar, alternar e configurar versões específicas do Python de forma global (para todo o sistema) ou local (para um diretório específico). Isso é especialmente útil ao trabalhar em diferentes projetos que requerem versões distintas do Python.

### Conceitos Importantes

- **Versão Global:** Define a versão do Python que será usada como padrão em todo o sistema, a menos que uma versão local seja especificada.
- **Versão Local:** Define a versão do Python que será usada em um diretório específico e seus subdiretórios, permitindo personalizar o ambiente para cada projeto.
- **Instalação de Versões:** Pyenv facilita a instalação de diversas versões do Python diretamente de fontes confiáveis, como o site oficial do Python.

---

## Instalação de Versões do Python com Pyenv

1. Instalar a versão 3.12.1 do Python:

    ```bash
    $ pyenv install 3.12.1
    ```

2. Instalar a versão 3.11.5 do Python:

    ```bash
    $ pyenv install 3.11.5
    ```

3. Instalar a versão 2.7 do Python:

    ```bash
    $ pyenv install 2.7
    ```

---

## Configuração de Versão Global do Python

Definir a versão global do Python para 3.12.1:

```bash
$ pyenv global 3.12.1
```

A configuração global será aplicada a todos os diretórios, exceto onde houver uma configuração local específica.

---

## Configuração de Versões Locais do Python

### Projeto Pandas
1. Navegar até o diretório do projeto:

    ```bash
    $ cd projeto_pandas/
    ```

2. Definir a versão local do Python para 3.12.1:

    ```bash
    $ pyenv local 3.12.1
    ```

3. Retornar ao diretório principal:

    ```bash
    $ cd ..
    ```

### Projeto Streamlit
1. Navegar até o diretório do projeto:

    ```bash
    $ cd projeto_streamlit/
    ```

2. Definir a versão local do Python para 3.11.5:

    ```bash
    $ pyenv local 3.11.5
    ```

3. Retornar ao diretório principal:

    ```bash
    $ cd ..
    ```

### Projeto Django
1. Navegar até o diretório do projeto:

    ```bash
    $ cd projeto_django/
    ```

2. Definir a versão local do Python para 2.7:

    ```bash
    $ pyenv local 2.7
    ```

3. Retornar ao diretório principal:

    ```bash
    $ cd ..
    ```

---

## Verificação de Versões Configuradas

Verificar a versão global atual do Python:

```bash
$ pyenv version
```

Resultado esperado:

```plaintext
3.12.1 (set by C:\Users\Administrador\.pyenv\pyenv-win\version)
```

Listar todas as versões instaladas e indicar a versão ativa:

```bash
$ pyenv versions
```

Resultado esperado:

```plaintext
  2.7
  3.11.5
* 3.12.1 (set by C:\Users\Administrador\.pyenv\pyenv-win\version)
```

---

## Verificação da Versão do Python

Confirmar a versão do Python em uso:

```bash
$ python --version
```

Resultado esperado:

```plaintext
Python 3.12.1
```

