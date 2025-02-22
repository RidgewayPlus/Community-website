# Joining the Windows Insider Program

This article covers how to join the Windows Insider Program to get builds of Windows 11.

## Joining the Windows Insider Program

> You must be logged onto a Microsoft Account to be able to join the Windows Insider program.
> This guide is intented to be followed from Windows 10 only, but allows you to receieve Windows 11 builds after joining.

1. Open the Settings app. You can do this by searching for it in the Start menu, pressing <kbd>Win</kbd> + <kbd>I</kbd>, or clicking the Settings button found above the Power button in Start. After that, open the **Update & Security** Section. 

<img src="./img/joining-windows-insider/settings-home.png" width="500px">

2. Click on **Windows Insider Program** on the sidebar to navigate to the sign up page.

<img src="./img/joining-windows-insider/settings-select-side.png" width="500px">

3. Click on the **Get Started** button to join the Windows Insider Program.

<img src="./img/joining-windows-insider/get-started.png" width="500px">

4. Click on **Register** to join the Windows Insider Program.

<img src="./img/joining-windows-insider/register.png" width="500px">

5. You will be prompted with a pop-up as shown below, click on **Sign Up**.

<img src="./img/joining-windows-insider/signup.png" width="500px">

6. Read the [Windows Insider Program Agreement](https://insider.windows.com/program-agreement) and the [Microsoft Insider Privacy Agreement](https://privacy.microsoft.com/privacystatement), then check **I've read and accept the terms of this agreement** if you agree. Then click **Submit**.

<img src="./img/joining-windows-insider/agree-and-submit.png" width="500px">

Shortly after that you should see a pop-up saying that you have successfully singed up for the Windows Insider Program. You now have to choose an account to signup as a Windows Insider.

<img src="./img/joining-windows-insider/link-an-account.png" width="500px">

7. Link an account to join the Windows Insider Program, then click **Continue**.

> You can choose any account to signup, but your personal Microsoft Account is recommmended.

<img src="./img/joining-windows-insider/account-link.png" width="350px">

8. Now select a channel to receive insider builds, then click **Confirm**. Here are some details on the details of the 3 channels:

| Channels                   | Description                                                                                                                                                                                                                                                               |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Dev Channel                | Ideal for highly technical users. Be the first to access the latest Windows 11 builds earliest in the development cycle with the newest code. There will be some rought edges and low stability.                                       |
| Beta Channel (Recommended) | Ideal for early adopters. These Windows 11 builds will be more reliable than builds from our Dev Channel. woth updates validated by Microsoft. Your feedback has the greatest impact here.                                             |
| Release Preview Channel    | Ideal if you want to preview and certain key features, plus get optional access to the next version of Windows before it's generally available to the world. This channel is also recommended for commercial users.                    |

<img src="./img/joining-windows-insider/channels.png" width="500px">

> if you don't see all 3 channels, you might be limited by your hardware. 

9. Read the [Microsoft Insider Privacy Statement](https://privacy.microsoft.com/privacystatement) and the [Microsoft Insider Program Agreement](https://insider.windows.com/program-agreement), then click **Confirm**.

<img src="./img/joining-windows-insider/agreement.png" width="500px">

10. Choose to *Restart Now* or *Restart Later*, then you will start receiving insider builds in *Settings> Updates & Security> Windows Update*. Have fun testing Windows Builds!

<img src="./img/joining-windows-insider/restart.png" width="500px">

## Leaving the Windows Insider Program

If you don't want to participate in the Windows Insider Program anymore, you can leave the program. Your computer will stay on the build that you are currently on until an official build that is newer than the build you have. You can also revert to an older build if you haven't deleted the Windows build and if you installed the build less than 10 days ago.

1. Open *Settings*, click on *Updates & Security*

<img src="./img/joining-windows-insider/settings-home.png" width="500px">

2. Click on **Windows Insider program**

<img src="./img/joining-windows-insider/settings-select-side.png" width="500px">

3. Click on **Leave the Insider Program**.

<img src="./img/joining-windows-insider/leaving-get-started.png" width="500px">

4. You will be redicted to an official website. Click on *Leave the Program now*.

<img src="./img/joining-windows-insider/leaving-the-program.png" width="500px">

> If you see *You must login to leave the program*, login on the top right corner of the website.

5. Click on **Stop receiving Insider Preview Builds**.

<img src="./img/joining-windows-insider/stop-receiving-builds.png" width="500px">

6. You should see *"This email address is not registered as a Windows Insider"*. If you don't see it, please redo step 3 and step 4.

## Troubleshooting

### Optional Diagnostics Data is diabled

If you see *"To manage the Windows Insider programme settings for your device and allow it to stay in the Windows Insider programme, you'll need to turn on optional diagnostic data."*, click on *"Go to Diagnostics & Feedback settings to turn on optional diagnostic data."*. 

<img src="./img/joining-windows-insider/optional-diagnos.png" width="500px">

> Photo source from [Minitool](https://www.minitool.com/news/how-to-join-windows-insider-program.html) 

Select **Optional diagnostic data** and return back the the Windows Insider Program page.

<img src="./img/joining-windows-insider/optional-diagnos-select.png" width="500px">

### Windows Insider Program Page not appearing

A registry key might be preventing the page from appearing in settings. Here is what you can do to fix it:

> Editing the registry incorrectly can cause major problems. Make sure you follow the instructions here exactly and don't proceed if anything is unusual.

1. Press <kbd>Win</kbd> + <kbd>R</kbd> and type in `regedit`, then press <kbd>Enter</kbd>

<img src="./img/joining-windows-insider/run.png" width="300px">

> You might be prompted with the User Account Control popup, click yes or enter an adminstrator's username and password to continue.

2. Go to the following registry key: `HKEY_LOCAL_MACHINE/SOFTWARE/Microsoft/WindowsSelfHost/UI/Visibility`

<img src="./img/joining-windows-insider/registry-1.png" width="500px">

> If the registry key does not exist, right click the key `UI` on the side bar and press **New > Key** and name it `Visibility`.

3. Right click and create a new 32-bit DWORD value named `HideInsiderPage` on the right hand side. Set the value to `0`.

<img src="./img/joining-windows-insider/registry-2.png" width="500px">

You may now close the Registry Editor window and restart your computer. The Windows Insider Program page should appear after the restart.

### Error Code 

You may see an error code while trying to register to be a Windows Insider. There are a lot of different error codes, so you should search it on the Internet or ask in [our Discord server](https://discord.gg/microsoft) for support (`#insiders` channel).