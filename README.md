https://liquity.ddns.net




HOW TO - 

https://github.com/liquity/liquity - DOCKER OR GITHUB 

I used docker - 

docker pull liquity/dev-frontend
docker run --name liquity -d --rm -p 3000:80 liquity/dev-frontend

 confirm running in browser or if config over vps then 
 
 ssh -L 3000:localhost:3000 USER@VPS.IP then 
 
 check web browser http://localhost:3000
 
 docker kill liquity
 
 Restart Docker with User Variables
 
 docker run --name liquity -d --rm -p 3000:80 \
  -e FRONTEND_TAG=(YOURETHADDRESS) \
  -e INFURA_API_KEY=(YOURINFURAKEY) \
  liquity/dev-frontend
  
  go to http://localhost:3000 (clear cache if need be) and do setup to set kickback rate. Try on Kovan or Ropsten before Main Net! 
  
  For free domain I used noip.com :) 
