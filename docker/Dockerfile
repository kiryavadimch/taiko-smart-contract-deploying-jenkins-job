FROM ubuntu:latest

RUN apt update && apt install -y && \
 apt install -y curl && \
 curl -L https://foundry.paradigm.xyz | bash && \
 foundryup && \
 curl https://sh.rustup.rs -sSf | sh && \
 forge init hello_foundry && \
 cd hello_foundry && \
 forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key $YOUR_PRIVATE_KEY src/Counter.sol:Counter