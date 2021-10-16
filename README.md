# uploadgram-tools
Simple tool to upload files to uploadgram from terminal

List of dependencies:
 - curl                                  — which is needed to make uploads
 - wc/du, awk                            — which usually come preinstalled
 - jq                                    — a simple command to parse json (needed for uploads)
 - libnotify                             — to get some status notifications
 - xclip                                 — to copy link/image to clipboard

## How to get it 
You can make a simple download by using
```bash
curl -O https://raw.githubusercontent.com/mrbooshehri/uploadgram-tools/master/uploadgram && chmod +x uploadgram
```
But let's suppose you want to install it for the whole system (which is a common use case)
```bash
curl -s https://raw.githubusercontent.com/mrbooshehri/uploadgram-tools/master/uploadgram | sudo bash -c 'cat > /usr/bin/uploadgram && chmod +x /usr/bin/uploadgram'
```
## How to use it
```bash
uploadgram <PATH_TO_YOUR_FILE>
```
