# log-in-system
I have used python 3 for the login authentication system, i have created it during the internship in Oasis Infobyte
# This is the code for log-in 
database=[]   # this is the container for the user-name and password 
datapass=[]
def register_user(username, password):
    if username in database:
        print("Username already taken. Please choose a different username. ")
    else:
        database.append(username)
        datapass.append(password)
        print("Registation Successful !")
# code for the log-in Registation
def main():
    while True:
        print("1. Register")
        print("2. login")
        print("3. Exit")
        choice = input("Please select an option: ")
        if choice == '1':
            username = input("Enter your username: ")
            password = input("Enter your password: ")
            register_user(username, password)
        elif choice == '2':
            username = input("Enter your username: ")
            password = input("Enter your password: ")
            if username in database:
                if password in datapass:
                    print("Login successful Welcome,"+ username +"!")
                else:
                    print("Incorrect password ! please try again.")
            else:
                print("Username not found. Please register first.")
        elif choice == '3':
            print("Exiting the system.")
            break
        else:
            print("invalid chioce. Please select a valid option. ")
main()        # Calling the decleared function
    ![Screenshot 2023-09-01 150015](https://github.com/vipweb09/log-in-system/assets/121581706/a3a2c76e-3235-41c4-880a-2a3fb055d00e)
![Screenshot 2023-09-01 145623](https://github.com/vipweb09/log-in-system/assets/121581706/508cbe0d-6bc6-465e-82a7-f22a2cb4dadb)
