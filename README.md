# iFlooder (Rootless)

iFlooder is a rootless iOS 16 tweak for the Messages app that adds a quick message-flooding/testing panel directly to an existing one-to-one conversation.

The tweak places an envelope icon in the top-right area of the Messages conversation header, beside the video-call button. Tapping the icon opens the iFlooder panel, where you can choose how messages are generated and start or stop a run.

## Features

- Built for **rootless iOS 16** jailbreaks.
- Integrates directly into Apple's **Messages** app.
- Adds an envelope button to the header of an existing one-to-one conversation.
- Sends one message request every **0.1 seconds** while a run is active.
- Includes **Fixed**, **Words**, and **Count** modes.
- Includes a dedicated **Stop** button to cancel any requests that have not yet been submitted.
- Automatically stops if you leave the conversation, close the iFlooder panel, or Messages becomes inactive.
- Includes an **Enabled** switch and **Respring** button in Settings.
- Does not require a separate companion app.

## Modes

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

## How to Use

To use iFlooder open an "existing" conversation and tap the envelope icon beside the video-call button. Choose Fixed, Words or Count, then start flooding. Messages send at 0.1 seconds. Stop cancels remaining requests; messages already handed to Messages cannot be recalled. Leaving the conversation or app also stops the flooding.

## Behaviour and Safety

Messages are submitted through the Messages app itself. Once a request has already been handed to Messages, iFlooder cannot recall it.

The Stop button only prevents requests that have not yet been submitted. The run also stops automatically when the active conversation changes, the iFlooder panel closes, or Messages is no longer the active app.

iFlooder only enables its sending panel when it can identify a supported existing one-to-one Messages conversation. It does not create a new recipient or conversation for you.

Use the tweak only in conversations and on devices where you have permission to perform testing. Rapid message sending can be disruptive and may be subject to carrier, iMessage, or service-side limits.

## Requirements

- iOS **16.0–16.x**
- Rootless jailbreak environment
- MobileSubstrate-compatible tweak injection
- PreferenceLoader for the Settings page

## Installation

Download the latest `.deb` from this repository and install it with your preferred rootless package manager, then respring when prompted.

After installation, open **Settings → iFlooder** to enable or disable the tweak and access the Respring option.

## Notes

- iFlooder is designed around the iOS 16 Messages/ChatKit interface.
- The envelope button appears only where the supported Messages conversation header is available.
- Compatibility may vary on heavily modified Messages setups or on unsupported iOS versions.

## Repository

This public repository is used for iFlooder release packages and project information.