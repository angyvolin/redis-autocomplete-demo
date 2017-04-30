# redis-autocomplete-demo

Redis autocomplete demo using ZRANGEBYLEX command. 
Autocomplete data was composed from 37000+ word definitions started from 'a', 'b' and 'c' letters taken from
[The Online Plain Text English Dictionary][1] as autocompletion dictionary.

Based on [antirez/search.php][2].

## Get up and running

### Installation

    git clone https://github.com/angyvolin/redis-autocomplete-demo.git
    composer install

### Populate redis with autocomplete data

    composer fixtures

### Run php web server

    composer run

### Customize redis options:

    REDIS_URL='redis://localhost:6379' composer run
    
or

    REDIS_URL='redis://user:pass@localhost:6379' composer run

[1]: https://www.mso.anu.edu.au/~ralph/OPTED/"
[2]: https://gist.github.com/antirez/11126283
