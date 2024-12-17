Server Management for Microservices Architecture
Directory Creation & Organization:
	 mkdir microservices_architecture && cd microservices_architecture/
	 mkdir microservices_architectureuser_service order_service inventory_service customer_service payment_service tax_service seller_service delivery_service storage_service help_service return_service digital_service
	 cd ./customer_service/ && touch Customer_{1..3}.txt
	 cd ../delivery_service/ && touch Delivery_{1..3}.txt && ls
	 cd ../digital_service/ && touch Digital_{1..3}.txt && ls
	 cd ../help_service/ && touch Help_{1..3}.txt && ls
	 cd ../inventory_service/ && touch Inventory_{1..3}.txt && ls
	 cd ../order_service/ && touch Order_{1..3}.txt && ls
	 cd ../payment_service/ && touch  Payment_{1..3}.txt && ls
         cd ../return_service/ && touch Return_{1..3}.txt && ls
	 cd ../seller_service/ && touch Seller_{1..3}.txt && ls
	 cd ../storage_service/ && touch Storage_{1..3}.txt && ls
	 cd ../tax_service/ && touch Tax_{1..3}.txt && ls
	 cd ../user_service/ && touch User_{1..3}.txt && ls
Move and Rename Files:
	 mv User_3.txt ../customer_service/
	 cd ..
	 cd customer_service/
	 ls
	 mv User_3.txt Customer_4.txt
	 Navigation & Listing Files:
	 cd ../microservices_architecture
	 tree
File Permissions Management:
	 touch config.txt
	 chmod 700 config.txt 
	 ls -all
Backup Files:
	 mkdir Backup
	 cp config.txt ./Backup/
	 cd Backup/
	 ls
	 Removing Files & Directories:
         cd ..
         cd user_service/
	 ls
	 rm User_1.txt 
	 ls
	 rm User_2.txt 
	 ls
	 cd ..
	 rmdir user_service/
Creating a Script for File Generation:
	 touch File_gntr.sh
	 nano File_gntr.sh
	 touch Component_{1..100}.txt
	 chmod 700 File_gntr.sh 
	 ./File_gntr.sh
Exploring File History:
	 history | tail -20
	 history | grep -e rm -e cp -e mv -e touch
System Monitoring:
 	 uptime
 	 ps aux
Ping Test & Network Verification:
 	 ping google.com
  	 ps
Search for Specific Files or Content:
	 find /home/administrator/MOHAMED_WASIM.R/Cloud_Computing_Essentials/microservices_architecture -name "Google.txt"
	 grep "13.9" Google.txt
Create a Directory for Each User:
	 mkdir User
	 cd User
	 mkdir user_customer user_delivery user_digital user_help user_inventory user_order user_payment user_return user_seller user_storage user_tax
Creating a Script for Directory Cleanup:
	 nano Delete_empty.sh
	 #!/bin/bash
         find /home/administrator/MOHAMED_WASIM.R/Cloud_Computing_Essentials/microservices_architecture -type d -empty -delete
         ./Delete_empty.sh
File Sorting & Management:
 	 ls -lhs
File Compression and Archive:
	 tar -czvf customer_service_backup.tar.gz customer_service
         tar -tzvf customer_service_backup.tar.gz 


