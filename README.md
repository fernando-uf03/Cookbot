# Cookbot

![Cookbot no CAD Creo Parametric](images/Cookbot.png "Cookbot")

O repositório destina-se à documentação do projeto do robô Cookbot, o qual é um robô manipulador do tipo PRR responsável por cozinhar batatas fritas em restaurante. Esse projeto foi desenvolvido na disciplina de Dinâmica de Sistemas Robóticos por estudantes da Escola de Engenharia de São Carlos (EESC-USP).

Em um projeto de engenharia, para a análise dinâmica de um robô manipulador, é fundamental a realização de simulações para verificar se o projeto é funcional e viável de ser fabricado na vida real. Para isso, esse repositório visa ser um guia ao leitor que deseja aprender como realizar a simulação do robô Cookbot.

Primeiramente, é importante ressaltar que o projeto foi desenvolvido em **ROS1 (distro Noetic 1.17.0)**. Por esse motivo, recomenda-se a instalação desta distro de ROS1 através do passo a passo disponível na página oficial ([Link](http://wiki.ros.org/noetic/Installation)). 

**Passo a passo para simulação:**

- Primeiramente, faça um clone deste repositório no diretório src (source) do workspace ROS de seu computador:
  ```
  git clone https://github.com/fernando-uf03/Cookbot.git
  ```

- Na raiz do workspace, isto é, dentro do workspace ROS, mas fora dos diretórios (src, devel e build, por exemplo), envie os seguintes comandos no terminal na seguinte ordem:
  ```
  catkin_make
  ```
  ```
  source devel/setup.bash
  ```

- Após isso, basta lançar o Cookbot no **Gazebo** e no **RViz**:
  - Para lançar o robô no **Gazebo**, use o seguinte comando
  ```
  roslaunch my_robot_urdf spawn_urdf.launch
  ```
  - Para lançar o robô no **RViz**, use o seguinte comando
  ```
  roslaunch my_robot_urdf display.launch
  ```

   
