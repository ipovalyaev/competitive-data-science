rebuild
	sudo docker build -t jupiter .

run 
	sudo docker run --network host -v ~/:/app/host/ -it jupiter
then inside 
	 cd /app/host/Syncable/competitive-data-science/ && jupyter notebook --allow-root

attach to existing container
	sudo docker exec -it <tab> bash
	to get token
 file:///root/.local/share/jupyter/runtime/nbserver-10-open.html
