# Ubuntu Server Configuration

1. After downloading the ISO and running it on VirtualBox, open it and install.
![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/877181d7-1614-40e5-a542-51d586387c9c)

2. After done install, reboot then enter the username and password you created.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/c80b9cfb-964d-42f8-b5ed-e73c28391b9e)

3. Type `sudo apt update`.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/cb5e7550-dd7a-4518-af41-62b213772d06)

4. Type `sudo apt install apache2`.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/265579ad-7382-47c4-b2b1-c04d8fe62824)

5. Type `sudo ufw app list` to check if everything is installed.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/e3922c89-8364-4610-ba5e-2df05009c44a)

6. Type `sudo ufw enable` and then `sudo ufw allow in "Apache Full" and "OpenSSH"`.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/b56f46e8-6585-4bcf-a8bd-536823f92f6a)

7. Type `ifconfig` to find the IP address; if not found, exit the virtual machine.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/59a6f17c-cbb8-4809-823e-6bd894aec940)

8. Set the network to bridge.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/0fcc4144-dd61-4c34-be75-4dcc42ae4c55)

9. Log in again, check the IP with `ifconfig`, and search the IP in Chrome. If successful, the display will look like this.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/faebc5ef-92f0-4e3d-a7a5-65d9aa2a89d1)

10. Remote using Ubuntu desktop.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/0621be8d-95e2-45e6-b592-da48926df373)

11. Remote using PuTTY in Windows.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/fbbae34c-bb37-4d54-991e-60aa87a1344b)

12. Remote using Windows CMD.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/72eb23fb-77f5-46d9-93ff-a9484bf14f74)

13. Remote using mobile SSH on a smartphone.
   
    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/000ac7e9-b9ad-4e8a-b1df-dc243bc601c0)

# Wordpress configuration

1. Log in as the root user to the system and update the system to refresh the repositories.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/0c4cb682-13f8-4639-9a1e-7c746313d442)

2. Install the MariaDB database engine to store your WordPress files.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/bafc200e-fa7e-4bbd-816e-522b545aa698)

3. Secure the MariaDB database engine and disable remote root login.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/8d46dcac-bc48-49df-869b-70393be47e02)

4. Install PHP.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/49efc50f-f447-4893-b23b-240c0e86a1a5)
   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/877941e0-08e3-44e1-9272-77ed193ba80f)


5. To confirm that PHP is installed, create and edit the info.php file.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/0ecce253-b4a4-47cf-9416-c5ea1450f00a)
   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/941b2d4a-03f3-4c68-9071-a408383e5d2c)


6. Check at ip address/info.php.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/442f742d-9039-4e75-a943-e63b08337624)

7. Log in to the MariaDB database as root and create a database to hold the data.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/6584d6b8-20a0-4718-99c7-547782d5c037)

8. Create a database for your WordPress installation.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/f05783e7-7b8b-4b47-a203-b4631e575f74)

9. Create a database user for your WordPress configuration.

   ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/b1a90e8b-8a36-4e4b-8e32-8bab82a05669)

10. Grant privileges to the user. Additionally, allow the user access to the database.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/eac55861-b7c9-4671-9883-f348444f0f58)

11. Exit the database.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/02433659-0333-4345-be52-3eff6ef04527)
    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/513aecf0-79a5-4edc-adba-b198fe60b21e)


12. Open your temporary directory and download the latest WordPress file.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/237219b3-1643-4ab3-8d8b-9a702b71fc88)

13. Extract the tarball compression, resulting in a folder named "wordpress."

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/329025ba-a4a8-40ae-9913-66f7f85ffcd1)

14. Copy the wordpress folder to this path.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/3b7de578-2ff0-41fc-9e5e-adba21e8b66b)

15. Run the command below to change the ownership of the 'wordpress' directory.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/d99e3853-e066-4bd1-b48f-fb5d23afccf8)

16. Change the permissions of the WordPress folder.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/455b42b3-fbce-42f6-8731-f9fcafe383e2)

17. Create an 'uploads' directory.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/c7bf9b64-b00f-4dec-a20f-c637e17e9a68)

18. Change the permissions of the 'uploads' directory, then reboot.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/828ece4f-d585-4b5e-bb92-8edea6cb7a07)

19. Change the directory to this path.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/b6fe0ec2-1e25-498d-adb7-c8fa44540572)

20. Edit the contents of this file so that the IP can be automatically updated.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/3c016f79-f597-47f1-9286-857d877dd3e5)
    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/092918a1-fed0-4177-b874-ba72fb0c238e)


21. Check for errors in the code with the command below; if none, then reboot.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/3b24016b-5448-4105-b87d-bf848bf59251)

22. Open Chrome and go to ip/wordpress, then create an account.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/33b6de3a-fd0d-4e9b-bf2d-c41f70e282f4)

23. After successful creation, you can start making posts in WordPress.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/60a0ab14-90b2-4e2b-8a58-fd9a794a5c0f)

24. Open the post tab to create a post. I have already created two posts here.

    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/5d0ce105-dcb5-4538-a6a4-6caf46d76666)
    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/f4a8b157-dd10-4705-b0cd-521e90f098b7)
    ![image](https://github.com/donavail/wordpress-ubuntu-server/assets/150001914/c6a8b83b-bf51-4734-80b6-4f59e611f3a3)


