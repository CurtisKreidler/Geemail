# Geemail
----
This project is a secure messaging client that is all run locally on one computer*.  This project uses the Crypto++ libary
for its clean salsa20 stream cipher and sha256 implementations. For the database we used sqlite with a sqlite3(called Sqlite3PP) 
wrapper class to simplify the DB read and writes

*note that this must be run on an Unix based computer becuase of the use of the dev/urandom system file in order to
compeletly randomly generate users salts based on the computers stored entropy. 

## Installation

1. Clone the repository
2. Install Crypto++ lib Instructions [Here](https://www.cryptopp.com/wiki/Linux)
3. Install sqlite3 with `sudo apt-get install sqlite3-dev`
4. The wonderful wrapper class is already include Link to their git repo is [HERE](https://github.com/iwongu/sqlite3pp)
5. Compile by running the `make` command
5. Run with `./geemail`


## Future Plans

* Make the Sala20 stream chiper IV dynamically generated to increase security
* Add in more error handling


## Credits

Collaborators: Adam Karpowich and Mike Mizikar
