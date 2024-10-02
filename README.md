# MakeyMakey
Projeto teclado/mouse.

O Makey Makey é uma ferramenta inovadora que permite aos usuários transformar praticamente qualquer objeto condutor em uma interface de controle interativa, como um teclado ou mouse.
O dispositivo físico é conectado ao computador via USB e permite que os objetos selecionados interajam com o computador, sendo interpretados como teclas de teclado ou cliques de mouse.

Versão do Python:
Para utilizar o Makey Makey com Python, qualquer versão recente do Python 3 pode ser usada. As bibliotecas dependem do tipo de projeto que você deseja desenvolver, mas a versão mínima recomendada do Python seria a 3.6 ou superior

Bibliotecas:
Para interagir com o Makey Makey e criar projetos em Python, as seguintes bibliotecas podem ser úteis, dependendo da funcionalidade que você deseja implementar:
Pygame: útil para criar interfaces gráficas e jogos interativos.

Instalação: pip install pygame
PySerial: para comunicação serial entre o Makey Makey e o seu computador (caso o projeto envolva isso).

Instalação: pip install pyserial
Keyboard: para mapear e monitorar eventos de teclado simulados.

Instalação: pip install keyboard
Tkinter (opcional): caso queira criar uma interface gráfica simples com botões e caixas de texto.

Instalação: Já vem embutido com o Python, sem necessidade de instalar.

Como Rodar/Instalar:
Passos para começar com o Makey Makey no Python:
Instalar Python:

Certifique-se de que o Python 3.6 ou superior esteja instalado no seu sistema.
Para verificar, execute no terminal: python --version ou python3 --version.
Instalar as bibliotecas necessárias:

Abra o terminal e execute os seguintes comandos para instalar as bibliotecas:
pip install pygame pyserial keyboard

Conectar o Makey Makey:

Conecte o Makey Makey ao seu computador via cabo USB.
Não é necessário instalar drivers adicionais para que ele seja reconhecido como um dispositivo de teclado ou mouse.
Escrever o código:

Crie um script Python que capture os eventos do Makey Makey
 (como pressionar uma tecla ou simular o toque de um objeto conectado ao dispositivo).

 Exemplo de script básico usando a biblioteca keyboard:

python
Copiar código
import keyboard

def on_key_event(e):
    print(f"Tecla {e.name} pressionada.")

# Adicionar o listener para capturar teclas pressionadas
keyboard.on_press(on_key_event)

# Manter o programa rodando
keyboard.wait('esc')  # Sai ao pressionar 'Esc'

Executar o código:

No terminal, navegue até o diretório onde o script está salvo e execute-o com:
python3 nome_do_script.py

Interação com o Makey Makey:

Use o Makey Makey para simular teclas de teclado ou mouse, e veja os eventos serem capturados no terminal ou em sua aplicação Python.
