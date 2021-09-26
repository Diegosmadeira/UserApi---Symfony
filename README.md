 API - LISTING AND CHANGING USERS
        
        Requirements: Server, Database Manager and text editor installed.
        Suggestion: XAMPP (https://www.apachefriends.org/download.html)
        Suggestion: Sublime-text (https://www.sublimetext.com/download)


        1. download the directories (by clicking on CODE -> DOWLOAD ZIP) into the directory where it will be used.

                    Unzip the directory.
                    Rename the directory to userApi                    
                   

        2.Configure your database in .env file on line 27:
        
          DATABASE_URL="(your database manager)://(database user):(database password)@127.0.0.1:3306/(database name)?serverVersion=13&charset=utf8"

          Example: DATABASE_URL="mysql://root:@127.0.0.1:3306/user_list?serverVersion=13&charset=utf8"
          
          
        3.Run on comand line(win + cmd on windows):
          Step 1. Write: cd (route to the project files directory)
         
          Example: cd C:\xampp\htdocs\userApi
          
          Step 2. Press Enter
          
          Step 3. Write symfony serve
          
          Step 4. Press Enter
          On this step you will get the development web server:
          
          Message Example:  
                            [OK] Web server listening                                                                                              
                            The Web server is using PHP CGI 8.0.8                                                                             
                            http://127.0.0.1:8000     
          
          Step 5. Open on Browser your Development Web Server.
          
          Example: http://127.0.0.1:8000     
          

        4. Use as you see fit
        
        
        5. To test the 'Update' and the 'Delete' User Specific method, click on Button 'Update Specic User' or 'Delete Specific User 'that it is going to open the Postman extension App  
         
        On Postman, to update a user you have to:
        
        step 1. Select the PUT method
        step 2. Write the Route: http://127.0.0.1:8000/users/(The number of ID you want to update)
        step 3. Click on Body
        step 4. select (x-www-form-urlencoded)
        step 5. Enter the key 'name' - '(Whatever value you want)'. 
        step 6. Enter the key 'email' - '(The email you want)'.
        step 7. Click Send.
        
        On Postman, to update a user you have to:
        step 1. Select the DELETE method
        step 2. Write the Route: http://127.0.0.1:8000/users/(The number of ID you want to update)
        step 3. Click Send.
