rebuild
	sudo docker build -t jupiter .

run 
	sudo docker run --network host -v ~/:/app/host/ -it jupiter
then inside 
	jupyter notebook --allow-root