FROM ubuntu:latest

RUN su apt-get update && su apt-get install -y && \
   su apt-get install -y curl && \
   curl -L https://foundry.paradigm.xyz | bash && \
   foundryup && \
   curl https://sh.rustup.rs -sSf | sh && \
   forge init hello_foundry && \
   cd hello_foundry && \
   forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key $YOUR_PRIVATE_KEY src/Counter.sol:Counter