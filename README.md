![image](https://github.com/user-attachments/assets/75f6a3ff-3670-42d9-a27a-5d03045dca83)




Hash Decoder
============

Overview
=========
This Python script is designed to decode various hash types using a wordlist. It is particularly useful for recovering passwords or other sensitive information that has been hashed.

Features
=========
Supports multiple hash algorithms (e.g., MD5, SHA-1, SHA-256, etc ).
Utilizes a wordlist for brute-force attacks.
Provides clear output indicating success or failure of the decoding process.

Requirements
============
Python 3.x
hashlib library (included in Python standard library)
A wordlist file containing potential passwords

Installation
============
Clone the repository or download the script.
Ensure you have Python 3.x installed on your machine.
Place your wordlist file in the same directory as the script.

Step 1. : Create venv python -m venv venv 
<br/>step 2. : Goto venv directory and run source bin/activate 
<br/>step 3. : Extract hash_Decoder tool in venv [gunzip hash_decoder1.0.0.tar.zp | tar -xvf hash_decoder1.0.0.tar]
<br/>step 4. : Goto directory hash_Decoder1.0.0
<br/>step 5. : pip install .   [this will install all the packages for hash decoder scipts]<br/>
step 6. : python3 setup.py\
step 7. : Now you can run these script   [python3 hashDecoder.py]<br/>


Usage
=====
To run the script, use the following command in your terminal:

Open In Editor
==============
python hashDecoder.py <hash_type> <hash_value> <wordlist_file>

Parameters
==========
<hash_type>: The type of hash you are trying to decode (e.g., md5, sha1, sha256).
<hash_value>: The hash value you want to decode.
<wordlist_file>: The path to your wordlist file.

Example
=======
python hashDecoder.py md5 5d41402abc4b2a76b9719d911017c592  wordlist.txt

python hashDecoder.py --md5 527bd5b5d689e2c32ae974c6229ff785 -w /usr/share/wordlists/rockyou.txt<br>
python hashDecoder.py --md5 527bd5b5d689e2c32ae974c6229ff785<br>
python3 hashDecoder.py --md5 527bd5b5d689e2c32ae974c6229ff785 -w /usr/share/wordlists/rockyou.txt -v


Output
=======
The script will output the decoded password if found, or a message indicating that the password was not found in the wordlist.
