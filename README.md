AM TV Remote - Fold-Out Keyboard Remote: Text-Entry Prototype

INFO 463 prototype for a smart TV remote with a fold-out keyboard, designed for older adults. This prototype tests one interaction: entering text on a TV (signing in, searching) with the keyboard remote compared with a standard D-pad and on-screen keyboard.

Live prototype: https://monicalli.github.io/AM-TV-Remote/

Files
index.html: the prototype (no installation required; phone pairing loads PeerJS from a CDN)
README.md: this file

How to run
Open the live link above, or download index.html and open it in a modern browser (Chrome, Safari, Firefox, Edge).
Use a laptop or desktop for the best experience. The facilitator panel sits at the top and the participant uses the remote on the right.

Phone remote
1. Open the live HTTPS page on the laptop, then select **Start phone pairing**.
2. Open the displayed link on the phone, or open the same page on the phone and enter the displayed code under **Have a pairing code?** Wait for both devices to say they are connected.
3. Use the phone's buttons. In condition A, changing the phone's screen orientation also rotates the remote; use **Unfold keyboard** to open its keyboard. If orientation is locked or does not change, use **Rotate remote** instead.
4. The laptop remains in charge of the TV, facilitator controls, and session log. One phone can connect at a time. If disconnected, use **Reconnect** on the phone. If the laptop still shows an old connection, select **Disconnect phone** before reconnecting. The laptop's own remote remains available as a fallback.

Pairing requires internet access to load PeerJS and reach its public signaling service. WebRTC connects the devices directly when the network allows it, but some networks block connections; test the actual venue network or try a shared hotspot. The public service and direct connections are not guaranteed. Local single-device use still works without pairing.

Treat the pairing code and link as private: anyone who has them can control the prototype while it is waiting for a phone. Pairing is intended for a supervised pilot, not for transmitting sensitive information. The link opens a remote-only view; it does not display the session log.
What it simulates

A virtual TV screen and a virtual remote. The only task flow built is:

Home → select YouTube → choose Sign in with this remote → type the target text → Done

Everything else (other tiles, phone sign-in) is intentionally not built and shows a short "not part of this test" message.

Condition A: Fold-out keyboard remote
Rotate remote turns the remote horizontal. The D-pad turns with it, so its directions remap.
Unfold keyboard opens the keyboard. These two buttons stand in for the physical gestures (Wizard of Oz).
Type by clicking the remote's keys or by using your laptop keyboard (Backspace to delete, Enter for Done).

Condition B: Baseline
The remote stays vertical.
Use the D-pad and OK to move across an on-screen keyboard and select keys. Select Done to finish.
Facilitator controls
Control	What it does
Condition	Switches between A and B (also resets the screen)
Task	Sign-in email or search phrase
Reset for next participant	Returns to the home screen with a clean state
Copy log as CSV	Copies all recorded runs for pasting into a spreadsheet
Data recorded per run
Time to first key (seconds): from the text screen appearing to the first character, which shows how quickly people find the keyboard
Typing time (seconds): first character to Done
Total time (seconds)
Keystrokes and backspaces
Whether the final text matched the target

The session log lives in the page only. It is cleared on refresh, so copy the CSV before closing the tab.