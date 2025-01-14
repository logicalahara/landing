# Controller Support

<Alert variant="warning">

You should disable Steam's controller support (or close Steam) before trying controllers on Plutonium.
Simply go to Steam Settings -> Controller -> General Controller Settings and **untick** the Checkboxes like shown below.

![disablesteamcontroller](/images/docs/controllers/U1bs5Z9.png)

</Alert>

## Xbox Controllers

Xbox controllers should be plug-and-play with all our games. Simply plug your controller into your computer and open Plutonium.

## PS4 Controllers

PS4 Controllers require a bit more setup.

1\. Download [DS4Windows](https://github.com/Ryochan7/DS4Windows/releases/latest). We recommend downloading `DS4Windows_VERSION_x64.zip`.

2\. Open the downloaded zip, and copy the `DS4Windows` folder to a safe place like your Documents folder.

3\. Open the extracted folder, then open `DS4Windows`

![img](/images/docs/controllers/sxik1Bs.png)

4\. If you get a message like this, then hit `Yes`.

![error](/images/docs/controllers/BEqRTW4.png)

4a\. Your browser should open, and you want to download the Windows x64 version.

![img](/images/docs/controllers/s2FRt73.png)

4b\. Open & install .NET.

5\. After installation, try DS4Windows again.

6\. Select `Appdata` for your SaveWhere path.

![img](/images/docs/controllers/3EJ1wzA.png)

7\. Install the ViGEmBus Driver.

![img](/images/docs/controllers/RHrY0Wu.png)

8\. Connect your PS4 Controller to your PC. If you are using bluetooth, follow the prompts inside DS4Windows

9\. Once connected, hit Finish on the Welcome to DS4Windows screen.

10\. Configure your controller and start DS4Windows in the main window.

11\. Go in game and see if your controller works!

## Switching Reload Action

Controller users are used to the X / Square button being used to reload but also held down to do the 'use' action.
On keyboard these are swapped to 2 separate keys, by default R for reload and F for use.

To swap it do the following:

1. [Open the console](/docs/opening-console)
2. Enter the following:
```cs
bind r +usereload
```
R should now be swapped to +usereload instead of +reload. Ensure your controller is mapped to the R button and you should be fine.

## Switching Triggers/Bumpers

You can switch the triggers and bumpers around by [opening the console](/docs/opening-console) and pasting this in:

```cs
bind BUTTON_LSHLDR "+speed_throw"; bind BUTTON_RSHLDR "+attack"; bind BUTTON_LTRIG "+smoke"; bind BUTTON_RTRIG "+frag"
```