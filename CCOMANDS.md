# ssh and gpg usage

* ssh-keygen -t ed25519 -C your_email@example.com
* ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
* start the ssh-agent in the background
* $ eval "$(ssh-agent -s)"
* > Agent pid 59566
* ssh-add ~/.ssh/id_ed25519

# gpg usage
* gpg --armor --symmetric --cipher-algo TWOFISH inputfile.txt
* gpg --armor --output decriptedFile --decrypt inputFile.txt.asc

# ffmpeg usage

## Add sound to a video
 * /c/Users/Public/PublicPrograms/ffmpeg-5.1.2-essentials_build/ffmpeg-5.1.2-essentials_build/bin/ffmpeg -i 2023week01-ex1a-test1a.m4a -i 2023week01-ex1a-test1a.mp4 -vcodec copy -acodec copy -shortest -map 0:a -map 1:v  combined1c.mp4

## Lower resolution
* /c/Users/Public/PublicPrograms/ffmpeg-5.1.2-essentials_build/ffmpeg-5.1.2-essentials_build/bin/ffmpeg -i 2023week01-js-review-array-methods.mp4 -s hd480 -strict -2 2023week01-js-review-array-methods-small.mp4
