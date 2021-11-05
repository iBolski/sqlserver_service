This contains the service script to start Sql Server in a WSL 2 instance. Since systemd isn't enabled in WSL 2, instead this script is used by Microsoft's own implementation of the old SYSV service daemon.

Copy the "mssql-server" script to the /etc/init.d folder.

	sudo cp mssql-server /etc/init.d

Navigate to the /etc/init.d and set it's permissions:

	sudo chmod 755 /etc/init.d/mssql-server

At this point, you can manually start and stop the service as follows:

	sudo service mssql-server start

	sudo service mssql-server stop

