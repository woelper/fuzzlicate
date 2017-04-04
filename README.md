# fuzzlicate
Find duplicate files locally or compare against a remote hashtable.


Examples:

Just find local duplicates:

    fuzzlicate --root-folder /home/someone/Documents
As above, and dump the result to 'ours.json'

    fuzzlicate --root-folder /home/someone/Documents --dump

Compare a remote dump with ours

    fuzzlicate --our-db ours.json --their-db theirs.json
