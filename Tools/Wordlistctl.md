# Wordlistctl

Script to fetch, install, update and search wordlist archives from websites offering wordlists with more than 6400 wordlists available.

[search wordlists](#search-wordlists)

[Fetch wordlists](#fetch-wordlists)

[list wordlists](#list-wordlists)


## Search Wordlists 

your OS is linux you have many wordlist in system so use search command and find wordlist in system 

    python3 wordlistctl.py search -l rockyou 
     
Search domain base wordlist in archives like

    python3 wordlistctl.py search facebook

     
## Fetch Wordlists

Search domain name base wordlist and downlods the wordlist in local systme use Fetch Command 

    sudo python3 wordlistctl.py fetch wordlist-name -d
     
     
## List Wordlists 

search wordlist like username, password, discovery, fuzzing, misc  use List Command like 

    python3 wordlistctl.py list -g usernames
    python3 wordlistctl.py list -g password
    python3 wordlistctl.py list -g discovery
    python3 wordlistctl.py list -g fuzzing
    python3 wordlistctl.py list -g misc
    
