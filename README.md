# Password Manager
Stores your passwords under AES256 encryption. Sensitive data is cleared from
RAM when the application exits.

Uses GTK+3.0 (to display GUI windows) and OpenSSL (to hash and encrypt data).
Requires a POSIX-compliant system, because I have used stuff not specified in
the C standard, but specified by POSIX.

# Usage
I have ceased development on this project. There is an extremely rare bug which
causes a segmentation fault while repeatedly performing all the actions
(changing, deleting and adding) in quick succession, and I am not able to
reproduce it. For all intents and purposes, the bug is random.
* Install the required libraries.
  * GTK+3.0: on Debian, enter the command `sudo apt install libgtk-3-dev`.
  * OpenSSL: on Debian, enter the command `sudo apt install libssl-dev`.
* Download/Clone the repository to some convenient location on your computer.
* Open a terminal window to that location.
* Enter the command `make run`.

The current passphrase is `q`, and you can change it. Some sample passwords are
already saved, and you can view them once you have entered the passphrase.

