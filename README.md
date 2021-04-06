https://liquity.ddns.net




## HOW TO - 

https://github.com/liquity/liquity - DOCKER OR GITHUB 

## DOCKER QUICKSTART ---


docker pull liquity/dev-frontend

docker run --name liquity -d --rm -p 3000:80 liquity/dev-frontend

## confirm running in browser or if setup via VPS then run below 
 
 ssh -L 3000:localhost:3000 USER@VPS.IP then 
 
## check web browser http://localhost:3000
 
 docker kill liquity
 
## Restart Docker with User Variables
 
 docker run --name liquity -d --rm -p 3000:80 \
  -e FRONTEND_TAG=(YOURETHADDRESS) \
  -e INFURA_API_KEY=(YOURINFURAKEY) \
  liquity/dev-frontend
  
 ## go to http://localhost:3000 (clear cache if need be) and do setup to set kickback rate. Try on Kovan or Ropsten before Main Net! 
 
 ## Copy files from docker to folder for static host
 
 docker cp liquity:/usr/share/nginx/html ./devui

## Host on Github!!
  
  ## For free domain I used https://noip.com :) 
