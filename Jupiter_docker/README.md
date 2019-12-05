rebuild
	sudo docker build -t jupiter .

run 
	sudo docker run --network host -v ~/:/app/host/ -it jupiter
then inside 
	 cd /app/host/Syncable/competitive-data-science/ && jupyter notebook --allow-root