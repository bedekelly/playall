PlayAll
=======

###A wrapper for tmsu and mplayer which allows creating playlists based on tag combinations. 

Requirements:
  * tmsu (with tags to use)
  * mplayer  
  * prettytable
  * python 3


Usage:

    playall [tag]...
  
    playall [tag=value]...
  
    playall --shuffle [tag | tag=value]...
  
    playall --search <"search term"> [tag | tag=value]...

    playall --generate [tag | tag=value]...  
  
--shuffle shuffles the files before being written to playlist. This is so that although the order is random, skipping forwards and backwards in mplayer does not disrupt the order.

--search allows for files which match a search term to be played first. If more than one file matches the search term, they will be added in the correct order (i.e. still in correct album order).#

--generate writes an mplayer-compatible playlist and does not play the files immediately.


For help using mplayer, use 'man mplayer'.
For help using tmsu, use 'tmsu help' or see http://tmsu.org.
