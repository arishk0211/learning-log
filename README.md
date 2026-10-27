# Learning Log — System and AI Essentials

## 1. Date and tools
**Date:** 27 October 2026  
**Tools:** FFmpeg and qrencode

## 2. What each tool is for
- **FFmpeg:** Processes video and audio, including extracting frames and creating GIFs.
- **qrencode:** Generates QR-code images from text or URLs.

## 3. Commands that worked
```bash
ffmpeg -i "/Users/arishks/workshop/Kungfu Panda.mp4" -frames:v 1 output.jpg

ffmpeg -i "/Users/arishks/workshop/Kungfu Panda.mp4" -t 5 ~/Desktop/short.gif

ffmpeg -i ~/Desktop/short.gif -vf "fps=10,scale=480:-1" ~/Desktop/final.gif

qrencode -o ~/Desktop/hello.png "Hello World"

qrencode -o ~/Desktop/github.png "https://github.com/arishk0211/first-project"
```

## 4. What broke and what fixed it
- **FFmpeg:** The output format or filter can fail if it is unsupported or misspelled. Check the error message and correct the format or filter name.
- **qrencode:** Leaving out the text to encode causes an error. Supply the text or URL after the options.

## 5. Five steps to remember
1. Read the tool's help or documentation.
2. Identify the command structure and required arguments.
3. Run a basic command and inspect the output.
4. Change one option at a time to improve the result.
5. Test the result and use error messages to troubleshoot.

## 6. What I want to try next
I want to extract video frames into separate images and learn more FFmpeg filters.
