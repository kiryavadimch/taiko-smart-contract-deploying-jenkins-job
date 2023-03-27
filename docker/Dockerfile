FROM ubuntu:latest

RUN apt install sudo
RUN sudo apt update && sudo apt install -y 
RUN    sudo apt install -y curl
RUN    curl -L https://foundry.paradigm.xyz | bash
RUN    foundryup 
RUN    curl https://sh.rustup.rs -sSf | sh
RUN   forge init hello_foundry
RUN  cd hello_foundry
RUN    forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key $YOUR_PRIVATE_KEY src/Counter.sol:Counter