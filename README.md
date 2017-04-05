# fuzzlicate
_Find duplicate files locally or compare against a remote hashtable._


Yet another file comparison tool?

Yes. If you have a subset of files in a different structure than on a remote machine, you can't just use rsync. Sometimes you want to know what data on your machine is already present elsewhere. Also, you can cache/--dump folder contents and perform fast comparisons against other folders. You can also share 'libraries' of files to other people whom may compare their files against.




Examples:

Just find local duplicates:

    fuzzlicate --root-folder /home/someone/Documents
As above, and dump the result to 'ours.json'

    fuzzlicate --root-folder /home/someone/Documents --dump

Compare a remote dump with ours

    fuzzlicate --our-db ours.json --their-db theirs.json


Known issues:
Both parties must use the same hash if comparing.
