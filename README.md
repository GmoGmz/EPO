ITESO EPO source code project 
===========
Autjor: Guillermo Gomez
ms684823@iteso.mx
guillermogomezmora@gmail.com

+52 1 331 892 3936

The instructions to make this compile on a system are the next:

1. Install nodejs 8.x
	curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
	sudo apt-get install -y nodejs

2. Modify file "credenciales.json"
	The part where it says "gmail" - "user" - "pass" you need to put a valid gmail address and a password

3. Create a directory and download the ITESO image:
	mkdir -p public/img
	cd public/img
	wget https://iteso.mx/lfportal-publico-theme/images/favicon.ico

4. Delete "package.json":
	cd ../..
	rm package.json

5. Create again the "package.json"
	npm init

6. Final steps:
	sudo apt-get update
	sudo apt-get install mysql-server
	mysql_secure_installation
