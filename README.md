# CS301-PROJECT
Project Created by Andrew Crews and Jacob Crews

- ! pip install poetry
- ! pip install nni # install nni
- ! wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip # download ngrok and unzip it
- ! unzip ngrok-stable-linux-amd64.zip
! mkdir -p nni_repo
! git clone https://github.com/microsoft/nni.git nni_repo/nni # clone NNI's offical repo to get examples
! ./ngrok authtoken 2GsgdqU7idVQyoxkN4NvUcpgm7p_3Rr5x28Sd6dzaxqgTA2nx
! nnictl create --config nni_repo/nni/examples/trials/mnist-pytorch/config.yml --port 5000 &
get_ipython().system_raw('./ngrok http 5000 &')
! curl -s http://localhost:4040/api/tunnels # don't change the port number 4040
