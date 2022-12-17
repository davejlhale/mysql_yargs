# Sequelize, nodejs, mysql , yargs

command line use  

node src/app.js --flags "values"

--flags
<...> user defined surround with "" if word breaks

--create movie --title <title> --director <director> --rating <int>
--create actor --name <name> --age <int> --nationality <nationality>
  (--title and --name required others optional)
  
  ## reading a full table
  --readAll actor
  --readAll movie
  --read actor
  --read movie
  
  
  --read actor --where "query string"
  --read movie --where "query string"
  the query string needs to be surrouned by ""
  the string is a key:value chain matching table keys
  eg
  --read actor --where "name:Ben Affleck"
  --read movie --where "rating:3"
  --read movie --where "rating:3,director:Ben Affleck"
  --read actor --where "nationality:english,age:32"
  


