# qaLink

Improves Steam Link VR streaming and unlocks H.264 on the Steam Frame

![qaLink's window while streaming](.github/images/qalink.png)

<img src=".github/images/client-pairing.jpg" width="49%" alt="qaLink Client in the headset, before pairing"> <img src=".github/images/client-streaming.jpg" width="49%" alt="qaLink Client in the headset while streaming">

## Requirements
- Windows
- SteamVR 2.18 or beta 2.19.3
- An NVIDIA GPU (AMD support is untested)
- A Steam Frame (other headsets, such as a Quest, get HEVC only for now. It's largely untested)
- qaLink Client: SteamOS 0.5.6, 0.5.7, 0.5.8, 0.5.9 or 0.6.0, in developer mode, with a password for your user

## Install
PC:
1. Download `qaLink-x.y.z.zip` from [Releases](https://github.com/jamess4rt/qaLink/releases/latest) and unzip it to
   a folder it can stay in, such as `C:\qaLink`.
2. Run `qalink.exe` and click **Install** in the Overview section. Restart SteamVR if it is running.
#
Steam Frame: open Konsole and run
```
curl -fsSL https://github.com/jamess4rt/qaLink/releases/latest/download/client.sh | bash
```

Type the pairing code it prints into the **qaLink Client** section on the PC and click **Pair**

Make sure to use the same qaLink version on the PC and the Frame.

## Uninstall
- PC: click **Uninstall** in the Overview section, then delete the folder.
- Frame: `sudo /etc/qalink-client/qalink-client uninstall`

## License
[PolyForm Strict 1.0.0](LICENSE.md): free for noncommercial use; no changes or redistribution. For commercial use,
contact the author on [Ko-fi](https://ko-fi.com/jamess4rt). Third-party licenses: `THIRD_PARTY_NOTICES.txt` in the
zip. Provided as is, without warranty.

qaLink is not affiliated with Valve, NVIDIA or AMD. Steam, SteamVR, Steam Link and Steam Frame are trademarks of
Valve Corporation; NVIDIA and NVENC of NVIDIA Corporation; AMD of Advanced Micro Devices, Inc.
