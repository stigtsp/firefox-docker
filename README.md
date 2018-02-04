https://developer.mozilla.org/en-US/Firefox/Headless_mode

docker build -t docker-firefox .

docker run -v $HOME/firefox-docker:/data  --rm -it docker-firefox /usr/bin/firefox -screenshot /data/screenshot.jpg https://stig.io/ -headless --window-size=480,1000


