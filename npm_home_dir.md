// setting up home npm global dir in path 

1. mkdir ~/.npm-global

2. npm config set prefix '~/.npm-global'

3. put in ~/.profile or ~/.bashrc 
    export PATH=~/.npm-global/bin:$PATH

4. update bash variables
    source ~/.profile or ~/.bashrc


