# VirusTotal API Hash Investigation
Python-based SOC automation tool that investigates IP addresses, domains, URLs, and file hashes using threat intelligence sources and generates an analyst-ready security report.
![image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/ac6e9848768043c5d6835aebacb572d375ce74de/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20190640.png)
In PowerShell create a folder for your project in VS Code by type mkdir SOC-IOC-Investigation-Automation and press enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/7599e6bda6e62c6d9d8c775df91294c79d434bfb/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20190640.png)
Next type cd SOC-IOC-Investigation-Automation and click enter
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/739fb5a308ecd946cab312e6a39a8a2f5c196c04/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20192440.png)

For this project, use a temporary change for just this PowerShell window rather than changing your whole computer's policy by typing Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass and press enter. 

Next activate the environment by typing .venv\Scripts\Activate.ps1 and press enter. 

You should see something similar to (.venv) PS C:\Users\eelve\SOC-IOC-Investigation-Automation>

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

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/bd81af2f7599a3c507a0495c5a352cf81aef7499/Screenshot%202026-08-31%20195714.png)

Press ctrl+s to save
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/95960e5d85805e4637fc079f51423c4b741232ea/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20195310.png)

Go back to PowerShell and type python main.py and press enter. You Should see

IOC INVESTERGATION TOOL 

----------------------
Testing SHA-256: .............................................

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/3fce67e177c7a7d7f576f8c082d4e4949b340d3b/Screenshot%202026-08-30%20224202.png)
Got to VirusTotal and copy your API Key
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/c4ef3e1bdc63de962e2427bc6b8fb097c16baebf/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20200220.png)
Open your .env file in Vs Code and type in your virustotal API Key after VT_API_KEY. Save it by pressing ctrl+s
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/7d3c0fb75ae8f50a97ec58fb6439e0fcec00bafa/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20200741.png)
Next, replace the contents of main.py with:

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/ee74312896931fbf79d8f38ec5ff9221b77734a4/Screenshot%202026-08-31%20193757.png)

Press ctrl+s to save
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/f429ff564c25f0319f02dd158faeb4eaa761f39e/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20201515.png)
Type python main.py and press enter. You should get 
API key loaded: True
API key length: 64
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/d9694352e2fd280ac87604b6b2dad21391668150/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20202041.png)
Right now, though, the main.py is still running the API-key test code, not the VirusTotal lookup code. Got back to Vs code and replace everything in main.py with this:

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/550f50604382fa77251d4ddaa89bff5de1a07af4/Screenshot%202026-08-31%20193835.png)

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/4a8e2a65bd720993b63c994f67b6dd8764c3251b/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20201649.png)
Go back to Powershell and type in python main.py and press enter. You should get something similar to 

VirusTotal Results
------------------
Malicious:  64
Suspicious: 0
Harmless:   0
Undetected: 3
![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/70128e9a2cb6288882682bce54470ad73dd5b04a/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20202041.png)
The next improvement is to make the tool interactive instead of hard-coding one hash. 

Go to Vs Code and change the hash_value =


hash_value = input("Enter SHA-256 hash to investigate: ").strip() 

Press ctrl+s

![Image alt](https://github.com/Kevinolee1/VirusTotal-API-Hash-Investigation/blob/3214b3c16f6bd89354def6875e560f4a4426c3e0/VirusTotal%20API%20Hash%20Investigation/Screenshot%202026-08-30%20202146.png)
Go back to Powershell and type in python main.py and press enter.

You'll get Enter SHA-256 hash to investigate:type in the hash you would like to investigate and press enter. 

Now your program will investigate whatever hash the analyst enters.
