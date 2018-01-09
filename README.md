# atomcat
A Go program with deep reinforcement learning and MCTS. It's a c++ implementation of the alphago-zero paper.
<br>

## Features
1. Self Play
2. Multi-thread search based on cpu cores
3. Deep neural network batch evaluation for board positions
4. CUDA support
<br>

## Dependency
Atomcat needs tensorflow c++ shared library to execute network inference.<br>
Download libtensorflow_all.tar.gz from https://mega.nz/#!PZsmCajD!9Opvihp6HgzS5CjG0fdU6OxGdwBGd5QqfAZTvbjvmgE (also you can build it from source), decompress, copy to directory /usr/lib.
```
$ sudo cp libtensorflow_all.so /usr/lib/
$ sudo ldconfig
```
<br>

## Hardware requirement
A nvidia GPU supports CUDA
<br>

## Run
Ubuntu 16.04 tested, currently windows platform is not supported.
```
1. start atomcat
$ ./atomcat

2. selfplay command
send self-play or selfplay command



   A B C D E F G H J K L M N O P Q R S T 
19 . . . . . . . . . . . . . . . . . . . 19
18 . . . . . . . . . . . . . . . . . . . 18
17 . . . . . . . . . . . . . . . . . . . 17
16 . . . + . . . . . + . . . . . + . . . 16
15 . . . . . . . . . . . . . . . . . . . 15
14 . . . . . . . . . . . . . . . . . . . 14
13 . . . . . . . . . . . . . . . . . . . 13
12 . . . . . . . . . . . . . . . . . . . 12
11 . . . . . . . . . . . . . . . . . . . 11
10 . . . + . . . . . + . . . . . + . . . 10
 9 . . . . . . . . . . . . . . . . . . . 9
 8 . . . . . . . . . . . . . . . . . . . 8
 7 . . . . . . . . . . . . . . . . . . . 7
 6 . . . . . . . . . . . . . . . . . . . 6
 5 . . . . . . . . . . . . . . . . . . . 5
 4 . . . + . . . . . + . . . . . + . . . 4
 3 . . . . . . . . . . . . . . . . . . . 3
 2 . . . . . . . . . . . . . . . . . . . 2   
 1 . . . . . . . . . . . . . . . . . . . 1   Black to play
   A B C D E F G H J K L M N O P Q R S T 

selfplay
```
<br>

## GUI
Sabaki is recommended, download Sabaki from http://sabaki.yichuanshen.de/ to ${SABAKI_HOME}
```
$ cd ${SABAKI_HOME}/Sabaki/dist/linux-unpacked
$ ./sabaki
```
