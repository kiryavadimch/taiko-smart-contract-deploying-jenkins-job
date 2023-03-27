FROM ubuntu:latest

# How to add env variable in dockerfile
# https://stackoverflow.com/questions/30494050/how-do-i-pass-environment-variables-to-docker-containers/30494145#30494145
# ENV YOUR_PRIVATE_KEY 

RUN apt update && apt install -y && \
   curl -L https://foundry.paradigm.xyz | bash && \
   foundryup && \
   curl https://sh.rustup.rs -sSf | sh && \
   forge init hello_foundry && \
   cd hello_foundry && \
   forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key YOUR_PRIVATE_KEY src/Counter.sol:Counter