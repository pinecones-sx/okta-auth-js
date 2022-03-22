# Demo of using okta with a single-page application
This is proof of concept to set up and configure a single-page application with Okta.

This was tested on a Windows 10 Pro computer and is provided as-is.  Results may vary.

To use this:
1. Clone the repo locally.
2. This application requires yarn & Node.js v 16.14.0.  If you already have these installed skip to step 5.
3. Install Node.js & yarn via Chocolatey in PowerShell.  You can do this using the Install-ChocoNodeYarn.ps1 script (by running unsigned or by manually entering the code from that ps1 file into PowerShell).
4. Navigate to the \\okta-auth-js\samples\generated\static-spa sub folder
5. From PowerShell run:
  ```
  yarn
  npm install --force
  yarn start
  ```
6. Run Google Chrome from command line with the following command (replaceing <PATH_TO_REPO> with the local path to the repo):
```
"C:\Program Files\Google\Chrome\Application\chrome.exe" --disable-site-isolation-trials --disable-web-security --user-data-dir="<PATH_TO_REPO>"
```
7. Navigate to http://localhost:8080 in Chrome
8. Enter the test username and password:
  ```
  username: demo.man@snipesstalone.com
  password: TestAccount.9274#
  ```
