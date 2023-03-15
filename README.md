# chrome-sync
## Install
    npm i && npm link
    
## Build docker chrome

        docker  run -d -p 3010:3000 --name chrome-clone-1 browserless/chrome
        docker  run -d -p 3011:3000 --name chrome-clone-2 browserless/chrome
## Run
    ts-node src/index.ts start -m "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" -c ws://192.168.1.20:3010 ws://192.168.1.20:3011

docker pull openstax/selenium-chrome:latest
