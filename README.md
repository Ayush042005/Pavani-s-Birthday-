# MY PROJECT TITLE IS PASSWORD MANAGER
#### THE VIDEO DEMO'S URL IS :
#### DESCRIPTION OF THE PROGRAM:
   This python is designed for the user to save all the user's passwords in one place locally
   so that in times of need user can retrieve those passwords easily. It provides the user
   functionalities which are generate ,check ,store , retrieve the password. the detail breakdown
   is as follows:

## Modules and Functions used:
  ** modules import **
     secrets: Used to generate cryptographically strong random numbers for password creation, ensuring the output cannot be predicted (unlike the standard random module).
     cryptography.fernet: A third-party library used for symmetric encryption. It handles the encryption of passwords before they are saved to the JSON file and decrypts them when retrieved.
     json: Handles the serialization and deserialization of the data, allowing the program to read and write the password vault as a structured JSON object.
     re: The Regular Expression module is used in validate_service_name to ensure input sanitization and in check_password_strength to detect specific character types (uppercase, digits, symbols).
     sys: Used to perform system-level operations, specifically sys.exit(1) to terminate the program securely if authentication fails.

   ** Funtions used **
     secrets.choice(): Used to securely select random characters from the character pool.
     secrets.SystemRandom().shuffle(): Used to shuffle the generated password characters to prevent predictable patterns.
     Fernet.encrypt() / Fernet.decrypt(): Methods from the cryptography library used to lock and unlock the password data.
     json.dump() / json.load(): Standard library methods used to serialize the dictionary data into a file and read it back.
     re.search() / re.match(): Regular expression methods used to find specific patterns (like digits or symbols) inside strings.
     sys.exit(): Used to safely terminate the program if authentication fails.

