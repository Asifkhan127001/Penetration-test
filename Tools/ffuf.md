# FFUF 

ffuf stands for Fuzz Faster U Fool. It's a tool used for web enumeration, fuzzing, and directory brute forcing.

## [Basic use](#basic-use)

## [Stop False result](#Filter HTTP response size)

## [Add Some Word in wordlist](#add-some-word-in-wordlist)

## [Extensions](#extensions)

## [Hide Status Code](#hide-status-code)

## [Find Status Code](#find-status-code)

## [Filter regexp](#Filter-regexp)

## [Filter HTTP response size](#Filter-HTTP-response-size)



## Basic Use

    ffuf -u http://example.com/FUZZ -w wordlist.txt -c 

## Filter HTTP response size

    ffuf -u http://example.com/FUZZ -w wordlist.txt -fs
    
## Add Some Word in wordlist

    ffuf -u http://example.com/FUZZ -w wordlist.txt:asif

## Extensions

    ffuf -u http://example.com/FUZZ -w wordlist.txt -e .php,.txt,.exe

## Hide Status Code

     ffuf -u http://example.com/FUZZ -w wordlist.txt -fc 403,302

## Find Status Code 

     ffuf -u http://example.com/FUZZ -w wordlist.txt -mc 403,302     

## Filter regexp

     ffuf -u http://example.com/FUZZ -w wordlist.txt -fr '/\..*'
     ffuf -u http://example.com/FUZZ -w wordlist.txt -fr ?


## Filter HTTP response size

















