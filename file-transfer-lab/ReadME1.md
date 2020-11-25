TCP file transfer instructions:
    - Get 2 terminals ready
        - First terminal: 
            - your going to want to run server first or you'll get an error when you run client first(ConnectionRefusedError: [Errno 61] Connection refused)
            - In the terminal command prompt change directories to "file-transfer-lab"  
            - In the terminal command prompt enter "Python3 Server.py" which will run the server
        - Second terminal:
            - In the terminal command prompt change directories to "file-transfer-lab"
            - In the terminal command prompt enter "Python3 Client.py >> [Your txt file name]"
            - Next the user will enter which file they want to transfer to receiver  
        
        * Make sure to have files already created with text for files they wish to transfer.
        * A file cannot be empty, wont crash but will get a warning message.
        * A file cannot send Ints, data needs to be in string format
        * Once the transfer is Successful it will let you know how many bytes were sent.
        * The server will recieve any file sent to it and store it in the same file location, it will 
            not accept duplicate file names, regardless of what's contained in them.
        * The server will create multiple threads to recieve files from multiple clients. 
        * The server can recieve several files at once, however it can only write to one file at a time.
         