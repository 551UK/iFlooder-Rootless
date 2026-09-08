# iFlooder (Rootless)

iFlooder is a rootless iOS 16.x tweak for the Messages app that adds a message flooder directly to an existing one-to-one conversation.

The tweak places an envelope icon in the top-right area of the Messages conversation header, beside the video-call button. Tapping the icon opens the iFlooder panel, where you can choose how messages are generated and start or stop a run.

## Features

- Built for **rootless iOS 16** jailbreaks and has been tested on my iOS 16 devices... May work on other iOS versions.
- Integrates nicely into Messages app.
- Adds an envelope button to the header of an existing one-to-one conversation.
- Sends one message every 0.1 seconds while flooding
- Includes three different modes like the original one from years ago... These are **Fixed**, **Words**, and **Count** modes.
- Automatically stops if you leave the conversation, close the iFlooder panel, hit stop or Messages becomes inactive.
- Includes an **Enabled** switch and **Respring** button in Settings.

## Modes inside the tweak and what they do.....

### Fixed

Repeats the exact text entered into the message box for each message in the run.

Example: if you enter `Test message`, each submitted message contains `Test message`.

### Words

Splits the text you enter into individual words and sends them one at a time in sequence, repeating the sequence as needed.

Example: entering `one two three` sends:

`one` → `two` → `three` → `one` → `two` → `three` ...

### Count

Automatically generates numbered messages starting from `1` and increasing by one for each message.

Example:

`1` → `2` → `3` → `4` → `5` ...

