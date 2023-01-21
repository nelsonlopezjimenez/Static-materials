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

