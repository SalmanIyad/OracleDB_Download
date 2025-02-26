# Oracle 19c & SQL Developer Install
Oracle 19c with SQL Developer Download and Installation Guide



# Download the Required Files

## Download Oracle 19c: 

  -  The Link of the Download Page: [Click Here](https://www.oracle.com/uk/database/technologies/oracle19c-windows-downloads.html).



 - In that Page Click the highlighted Link [if you are using windows] 

![1](https://user-images.githubusercontent.com/110406908/222976303-86ad65cb-0211-4293-8073-da22768cda1e.png)

- If you got this dialog box click Download WINDOWS.X64_193000_db_home.zip

![2](https://user-images.githubusercontent.com/110406908/222976652-e77b40ad-4a9b-4760-b8a5-2044b1f04a49.png)
 ```
 - You should have an account on oracle [Create One if you don't :)]
 ```
- Now you may be forwarded to the [sign in page](https://login.oracle.com/mysso/signon.jsp), Sign in and the Download will start automatically.



## Download SQL Developer: 

-  The Link of the Download Page: [Click Here](https://www.oracle.com/database/sqldeveloper/technologies/download/).

 - In that Page Click the highlighted Link [if you are using windows], and you'll find your version for other operating Systems below.
![3](https://user-images.githubusercontent.com/110406908/222978191-6bca98fc-6d3b-49cd-9349-f1881a8c4aee.png)
- If you got this dialog box click Download Button and the Download will start automatically.
![4](https://user-images.githubusercontent.com/110406908/222978662-d84eb411-3f2d-441c-9690-ba950825e511.png)


# Installation 

## Setting Up Orcale 19c
```
Important: You should Have an internet connection to get this DONE!
```
- First You Should have this tow Files on your machine, Then Follow the following instructions: 

    ![image](https://user-images.githubusercontent.com/110406908/222979929-e43d2cdb-b87d-4507-8df9-8fafd7ab0dd6.png)

- Go to your C Drive and create new folder with name `app`.

    ![image](https://user-images.githubusercontent.com/110406908/222979598-f500aeed-1c7e-4735-a4a7-39a27328cc46.png)

- Inside `app` folder, Extract the `WINDOWS.X64_193000_db_home.zip` file into `db_home` folder.

    ![image](https://user-images.githubusercontent.com/110406908/222979707-cce90b9d-4478-4494-85b9-d7367fa60646.png)

- After extracting is complete, Run the `Setup.exe`

    ![image](https://user-images.githubusercontent.com/110406908/222979843-4c977040-9636-461e-8a41-4ee09f062cee.png)

- The Setup will start launching, just wait.

    ![image](https://user-images.githubusercontent.com/110406908/222980304-47987a4c-60a6-44f4-988f-74d39a9b5ae9.png)

- Now choose the same settings in the ScreenShots below and click `next` every time..

    ![image](https://user-images.githubusercontent.com/110406908/222980431-27862bdc-358f-4b6b-a841-06546dc47d41.png)

    ![image](https://user-images.githubusercontent.com/110406908/222980548-c2262445-5f86-472d-8e29-250fd7dcaf16.png)

    ![image](https://user-images.githubusercontent.com/110406908/222980556-b0f296a8-cca1-4fa4-8cd1-dd7321acb007.png)

- Now The screen below is very important, Check these out: 
    - Oracle Home: `C:\app`, as Default.
    - Database file location: `C:\app\oradata`, as Default. 
    - Global database name: `orcl`, this could be something else by Default, Make Sure to change it to `orcl`. 
    - Password: Set it any Password you want, such as `111` or `000`, But remember it.
    - Confirm password: just repeat your password.
    - Check on Create as Container database.
    - Plugguble database name: `orclpdb`.
    - Then click `next`.

    ![image](https://user-images.githubusercontent.com/110406908/222980656-3cb15b5b-5e8a-448a-ba3d-57150cd3b26e.png)

```
    As you see down in Messages Section, it shows that the password is weak, just do not worry.
 ```

- It shows that the password is weak, Don't Care, Click `Yes`.

    ![image](https://user-images.githubusercontent.com/110406908/222981483-a37aaf54-b53a-41c6-9922-17c66d8e645a.png)


- Now Click `Install`.

    ![image](https://user-images.githubusercontent.com/110406908/222981688-148714b0-5902-41e3-bcfc-a6f9e4bfb84f.png)


- If this Window popped up, just click `Allow access`, and wait until the installation finishes. 

    ![image](https://user-images.githubusercontent.com/110406908/222981748-588bb582-eaa9-4f57-a52a-cb0043f41106.png)

- Now to test the database is successfully installed or not, just copy the highlighted link and click `close`.

    ![image](https://user-images.githubusercontent.com/110406908/222982108-a65817a5-be17-447e-947f-9a9652369c68.png)
    
- then paste it into the browser and log in as: 
    - Username: `sys`.
    - Password: the password you created while setup, "in my case `111`".

    ![image](https://user-images.githubusercontent.com/110406908/222982202-7e467beb-5daa-46ba-ad3c-9bc053f06198.png)


- That should shows this Dashboard. 
    ![image](https://user-images.githubusercontent.com/110406908/222982517-567aa8b0-c80b-47d6-aa26-d00244a2c217.png)


## Setting Up SQL Developer

- First go to this path `C:\app\db_home\network\admin` and open `tnsnames.ora` file with Notepad.

    ![image](https://user-images.githubusercontent.com/110406908/222984667-242bc2d2-dbe2-4c3d-a581-8e5fb7097361.png)

- Copy this selected part and paste it below it directly.

    ![image](https://user-images.githubusercontent.com/110406908/222984758-5f0da643-008c-4346-a3d8-308921196057.png)

- Edit `ORCL` words to `ORCLPDB` as following.
    ![image](https://user-images.githubusercontent.com/110406908/222984913-95c5910a-71cc-432b-85f0-0366f475bab1.png)
    #
    ![image](https://user-images.githubusercontent.com/110406908/222984924-43256083-fce1-48fc-8f04-f1a3899ec07b.png)

- Save the file with `Ctrl + S`, and close it.

- Open Command Prompt (CMD), By searching for it, Or press `Windows logo + R` in the Keyboard and type `cmd`, then click `OK`.

    ![image](https://user-images.githubusercontent.com/110406908/222983004-3c6afcfa-5070-42f3-98ef-185c8daab557.png)


- Type `sqlplus` and hit `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222983203-5e069db0-a458-40f5-8db3-09f66f41b908.png)

- Type `/ as sysdba` in the user-name field and hit `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222983572-c8397a8e-7fa0-40d0-b747-c854bc7412ac.png)

- OR type `sys as sysdba` in the user-name field and hit `Enter`, then type your password [`111` in my case] and hit  `Enter`.

```
    (: Don't Worry, The password will not appear while typing..
```
- Type `alter session set container = orclpdb;` to change the container database to 'orclpdb', and hit  `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222983949-ab581493-1c0b-4506-9da9-ac0ed2c88030.png)


- Type `alter user hr identified by hr account unlock;` to unlock the hr database user, and hit `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222984084-2245089a-002f-4894-9159-6e65f84bbd46.png)

 - If you faced any problem here type ```startup;``` and try again.


- Type `conn hr/hr@orclpdb;` to Connect to the `hr` user that has `hr` password, and hit `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222984147-205ddf98-7134-44be-9f4b-efdfdecd6c13.png)

- Type `alter pluggable database orclpdb save state;` to save the pluggable database state, and hit `Enter`.

    ![image](https://user-images.githubusercontent.com/110406908/222985429-f0cab04e-4de7-4cb2-a2ea-fd9f42758e49.png)
    
#

 - Commands Summary: 
    ```
    sqlplus / as sysdba
    alter session set container = orclpdb;
    alter user hr identified by hr account unlock;
    conn hr/hr@orclpdb;
    alter pluggable database orclpdb save state;
    ```
#


- Back to the second `.ZIP` file.

    ![image](https://user-images.githubusercontent.com/110406908/222985680-068d1c97-0efe-4a78-8b29-3b34e64158d7.png)

- Extract it into the `app` folder.

    ![image](https://user-images.githubusercontent.com/110406908/222985756-7dfd4407-a631-4e04-8b5c-f1bf09a6be51.png)

- Inside the extracted `sqldeveloper` folder, go down to `sqldeveloper.exe`, right click on it and send it to the desktop "as a shortcut".
    
    ![image](https://user-images.githubusercontent.com/110406908/222986008-424cd1fb-dd11-46cc-a0f9-9635ac760b4f.png)

- Run the sqldeveloper from your desktop shortcut.

    ![image](https://user-images.githubusercontent.com/110406908/222986086-d8d5fd64-b1e5-4778-b758-1031490324ae.png)

- From the left up corner click the green `+` sign to ad a connection.

    ![image](https://user-images.githubusercontent.com/110406908/222986156-5c300a87-178b-4f47-8380-d249e4bbf8fb.png)

- In this Window the `Name`, `Username` and `Password` are `hr`, then Check the `Service name` and set it to `orclpdb`.
    
    ![Untitled](https://user-images.githubusercontent.com/110406908/222986564-a1647b8f-4b00-4380-983c-23765459c16f.png)


- Click `Test` Button and it should be `Status: Success` showed in bottom-left of the window.
 
    ![image](https://user-images.githubusercontent.com/110406908/222986918-a2f7ace4-d81a-4e4f-ab45-f91d4493db29.png)

- Then click `Connect` Button.

    ![image](https://user-images.githubusercontent.com/110406908/222987174-e0406c31-caff-4d31-956a-9597cf6527cd.png)

- Here you can write `SQL Commands` and Run it using the green run Button on the top toolbar.

    ![image](https://user-images.githubusercontent.com/110406908/222987122-89a9a527-0e46-4f43-a493-fdb9dc4ea356.png)
# Authors

- [@SalmanIyad](https://www.github.com/SalmanIyad)


## Good Luck!

