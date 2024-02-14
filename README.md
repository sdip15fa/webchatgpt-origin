https://github.com/interstellard/chatgpt-advanced has gone closed-source. I would like to re-publish the open source version.


See [build from source](#build-from-source) for build instructions.

<div align="center">
<h1>WebChatGPT Origin</h1>


This browser extension `adds web access` capability to [ChatGPT](https://chat.openai.com/). Get much more relevant and up-to-date answers from the chatbot!

## Manual installation

  Don't forget to disable the extension installed from the Web Store while you're testing manually installed version.
  
  ### Chrome, Microsoft Edge, etc.
  1. Download the prebuilt chrome zip file from [here](build).
  2. Unzip the file.
  3. Open `chrome://extensions` in Chrome / `edge://extensions` in Microsoft Edge.
  4. Enable developer mode (top right corner).
  5. Click on `Load unpacked` and select the unzipped folder.
  6. Go to [ChatGPT](https://chat.openai.com/chat/) and enjoy!

  ### Firefox
  1. Download prebuilt firefox zip file from [here](build).
  
  #### Temporary installation, in official Release or Beta
  1. Go to `about:debugging#/runtime/this-firefox`.
  2. Click `Load Temporary Add-on` button, then select the zip file you re-zipped.

  #### Persistent installation, in Nightly or Developer Edition
  1. Open Firefox, go to `about:config` and set `xpinstall.signatures.required` to `false`.
  2. Go to `about:addons`
  3. Click on the gear icon in the top right corner of the Add-ons page and select `Install Add-on From File`.
  4. Select the zip file and click open.
  5. Firefox will prompt you to confirm the installation of the addon. Click Install.
  6. The addon will be installed and will appear in the list of installed addons on the Add-ons page.
  7. Go to [ChatGPT](https://chat.openai.com/chat/) and enjoy!


## Build from source

1. `git clone https://github.com/qunash/chatgpt-advanced.git`
2. `npm install`
3. `npm run build-prod`
4. Grab your zip extension from `build/` folder

<br>

## FAQ

### Why is the extension asking for `access to all websites` permission?
The extension requires access to all websites because there is no backend server to process web requests, and everything happens locally in the browser. There are two modes: web searching, and extracting webpage text from URLs. Web searching requires access to the search engine, while URL text extraction requires access to any website. This is why the `access to all websites` permission is required.

### The extension does not work, the toolbar does not show up. What can I do?
Some other ChatGPT extensions are known to interfere with WebChatGPT. If you are experiencing issues with the toolbar not showing up, please try disabling any other ChatGPT extensions that you have installed and reloading the page.

### Do you collect any data?
No, the extension does not collect any user data or analytics.
