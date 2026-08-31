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
