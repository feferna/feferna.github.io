---
title: "Uma introdução ao Robot Operating System (ROS)"
date: 2016-03-02
permalink: /posts/2016/03/introducao-ao-ros/
author: Francisco Erivaldo Fernandes Junior
excerpt: "Entenda o que é o ROS (Robot Operating System) e como ele pode facilitar a comunicação entre os módulos do seu robô."
tags: 
- ros
- robótica
- linux
- middleware
- embarcados
---

>  **Nota de atribuição:**  
> Este artigo foi originalmente publicado no site [Embarcados](https://embarcados.com.br/uma-introducao-ao-robot-operating-system-ros/) em 2 de março de 2016.  
> Este conteúdo está republicado aqui com o objetivo de arquivamento e acesso contínuo.


# Uma introdução ao Robot Operating System (ROS)

Este post faz parte da série ROS (Robot Operating System). Leia também os outros posts da série:

- Uma introdução ao Robot Operating System (ROS)
- Entendendo os nós do ROS
- Entendendo as mensagens e tópicos do ROS
- Criando um “Hello World” no Robot Operating System (ROS)

---

Se você está construindo um robô que possui diferentes módulos — como câmera, sensores laser, GPS, etc. — que precisam se comunicar entre si, você já deve ter se perguntado se existe uma maneira mais fácil de realizar essa comunicação. A resposta é sim!

Para facilitar a comunicação entre diferentes módulos, você pode utilizar o **Robot Operating System (ROS)**. Usando o ROS, é possível criar uma arquitetura de processamento de dados em paralelo para controlar seu robô.

Por exemplo, imagine que você precise realizar cálculos pesados de processamento de imagem, mas o PC embarcado do robô não é suficiente. Você pode resolver esse problema criando um nó ROS em um PC mais poderoso e se comunicar via TCP/IP com o robô.

---

> “ROS é um conjunto de bibliotecas e ferramentas que te ajudam na construção de aplicações para robôs. De drivers até algoritmos de última geração e com poderosas ferramentas de desenvolvimento, ROS possui o que você precisa para seu projeto de robótica. E o melhor de tudo: ROS é OpenSource.”

---

## Conceitos básicos

ROS possui uma arquitetura simples. Em uma rede com máquinas rodando ROS, sempre existe uma máquina conhecida como **MESTRE**, que executa o comando `roscore` para inicializar os serviços necessários à comunicação entre os nós ROS.

Um **nó ROS** é basicamente um executável. Assim, é possível ter nós rodando em diferentes máquinas na mesma rede. A comunicação entre nós é feita via TCP/IP.

Cada nó pode publicar ou subscrever em **tópicos**, que funcionam como variáveis compartilhadas. Um nó pode escrever valores (publicar) ou ler valores (subscrever) desses tópicos. Assim, múltiplos nós podem se comunicar entre si.

### Comunicação entre nós

![Figura 1: Ilustração da comunicação entre nós ROS. Exemplo: o nó `/camera_base_link` envia dados pelo tópico `/tf` para o nó `/camera/camera_nodelet_manager`.](/images/blog/ros/fig1_ros_nos.png)

## Criação de pacotes

ROS oferece ferramentas para criação de pacotes em C++ e Python. Cada pacote pode conter um número arbitrário de nós. Para isso, é necessário ter conhecimentos básicos em **CMake** e terminal Linux. A criação de pacotes será abordada em tutoriais futuros.

---

## Instalação do ROS (Robot Operating System)

Infelizmente, o ROS funciona apenas em Linux e macOS. Existe um projeto para portar ROS para Windows, mas está desatualizado.

Este tutorial mostra como instalar a versão **ROS Indigo** no **Ubuntu 14.04 (64 bits)**.

### 1. Adicione o repositório ROS:

```bash
sudo sh -c 'echo "deb https://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

### 2. Adicione a chave GPG:

```bash
sudo apt-key adv --keyserver hkp://pool.sks-keyservers.net --recv-key 0xB01FA116
```

### 3. Atualize os pacotes:

```bash
sudo apt-get update
```

### 4. Instale o ROS Desktop completo:

```bash
sudo apt-get install ros-indigo-desktop-full
```

### 5. Inicialize o `rosdep`:

```bash
sudo rosdep init
rosdep update
```

> ⚠️ Sempre execute o `rosdep` como **usuário comum** (não como `root`) para evitar problemas de permissão.

### 6. Configure o ambiente:

```bash
echo "source /opt/ros/indigo/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

---

Pronto! Agora você tem o ROS instalado em sua máquina Linux. Nos próximos tutoriais, você vai ganhar mais familiaridade com os conceitos do ROS.

---

## Fontes

- [Website oficial do ROS](http://www.ros.org)
- [Tutorial em inglês sobre instalação do ROS](http://wiki.ros.org/indigo/Installation/Ubuntu)
- [Visualização de nós e tópicos no ROS](http://wiki.ros.org/rqt_graph)
