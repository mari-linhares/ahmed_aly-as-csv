# ahmed_aly As CSV

Python script that takes an [ahmed-aly](http://ahmed-aly.com/) standing and returns a csv with the submissions information.
This was tested only on Linux.

# What will I need in order to run it?

Some python libs:
- selenium
- cssselect
- csv
- lxml.html

And some internet connection will help haha :smile: (but really, you'll need it). Algo I'm using mozilla as browser, you can change it if you want, just change the webdriver line in [this file](https://github.com/mari-linhares/ahmed_aly-as-csv/blob/master/utils/webConnection.py).

# Ok, but how do I run it?

Run it on shell:

`$python runApp.py <ID of the standings> -o <name/path of the output>`

If the name/path of the output isn't explicit the output will be `<Standings name>.csv`

# How is the output file?

Username | Ranking | Country | Number of Solved Problems| P1 - url | P2 - url | P3 - url | ... | PN - url|
-------- | --------| --------| -------------------------| ---------| ---------| ---------| ----| --------|
user1    |    1    |  Brazil |              3           |     1    |     1    |     1    | ... |     0/0 |
user2    |    2    |  India  |              2           |     0/0  |     0/0  |     1    | ... |     1   |
user3    |    3    |  Russia |              2           |     0/8  |     1    |     0/0  | ... |     1   |
...      |    ...  |  Brazil |              1           |     0/0  |     1    |     0/7  | ... |     0/54|
usern    |    n    |  Brazil |              0           |     0/100|     0/0  |     0/0  | ... |     0/0 |
