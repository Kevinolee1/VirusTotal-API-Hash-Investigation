# VirusTotal API Hash Investigation
Python-based SOC automation tool that investigates IP addresses, domains, URLs, and file hashes using threat intelligence sources and generates an analyst-ready security report.
![image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/ac6e9848768043c5d6835aebacb572d375ce74de/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20190640.png)
In PowerShell create a folder for your project in VS Code by type mkdir SOC-IOC-Investigation-Automation and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/7599e6bda6e62c6d9d8c775df91294c79d434bfb/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20190640.png)
Next type cd SOC-IOC-Investigation-Automation and click enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/739fb5a308ecd946cab312e6a39a8a2f5c196c04/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20192440.png)
For this project, use a temporary change for just this PowerShell window rather than changing your whole computer's policy by typing Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass and press enter. Next activate the environment by typing .venv\Scripts\Activate.ps1 and press enter. You should see something similar to (.venv) PS C:\Users\eelve\SOC-IOC-Investigation-Automation>
![image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/b4b2d57d2c53a41583ad1d94d49c555e9131abd1/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20192440.png)
Now install the two packages by typing python -m pip install requests python-dotenv and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/f172ec702867342f8023f4ac4d4b63c08b21fea2/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20192858.png)
Then create the main project file by typing New-Item main.py and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/2f544ab5825f735612c27572c679489ea452651f/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20193130.png)
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/cfc951b68193dbd311f7af92f2d21c5e238fd1c1/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20193248.png)
Also create these files by typing New-Item .env,New-Item .env.example, New-Item .gitignore, New-Item requirements.txt and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/e7609b11fc96aa960e39744e393b2222a59951ab/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20193948.png)
python -m pip freeze > requirements.txt and press enter to run. Next, open the project folder in VS Code by typing code . and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/da1e1c8a0182a91a869cdb5e97d63527c74f95f3/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20194352.png)
Then open main.py in VS code and type in 

import requests

hash_value = "type in the hash value"

print("IOC Investigation Tool")
print("----------------------")
print(f"Testing SHA-256: {hash_value}")
Press ctrl+s to save
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/95960e5d85805e4637fc079f51423c4b741232ea/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20195310.png)

Go back to PowerShell and type python main.py and press enter. You Should see

IOC INVESTERGATION TOOL 

----------------------
Testing SHA-256: .............................................
Got to VirusTotal 
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/c4ef3e1bdc63de962e2427bc6b8fb097c16baebf/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20200220.png)

