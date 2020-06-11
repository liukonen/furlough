# Day 48
 
Watched the latest episode of TheDotNetDocs live, and refactored / rebuilt NATS standard with the LiteDB DB option, removing all code for SQL Lite. LiteDB is the first NoSQL DB I've worked with, and Im impressed with its Code forward approch. 
Not sure why I was having the problems I was with SqLite... it says it's cross platform, but I couldn't get the DLL's to load or work. LiteDB just worked, and I don't have to ship around a DB file, as it can construct it on the fly. 