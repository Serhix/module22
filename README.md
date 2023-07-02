# Phone book assistant
This project is a personal assistant with a command line interface.

## Installation
To start a Docker container, you need:
- download content from GitHub
- execute in the terminal: docker build [OPTIONS] PATH | URL | - (docker build -t assistant .)
- execute in the terminal: docker run [options] image: tag [command, args] (docker run -ti assistant)

## Usage (comand)
- Hello - start of work, greetings
- show all - displays the entire phone book with numbers and birthdays (N contacts on one page)(example: show all 10)
- info - displays the phone number and birthday of the selected contact (example: info ContasctName)
- add - adds a phone for a contact (example: add ContasctName 0980000000)
- birthday - adds a birthday for a contact (example: birthday ContasctName dd.mm.yyyy)
- change - changes the phone number for the specified contact if the number and contact exist (example: change ContasctName Phone)
- delete - deletes the phone number for the specified contact if the number and contact exist (example: delete ContasctName Phone)
- when birthday - outputs the number of days until the next birthday (if the data is available) (example: when birthday ContasctName)
- find - search by matches in the address book, by several digits of a phone number, or by several letters of a name (example: find 38098)
- close, exit, good bye - completing work with the assistant, saving contacts