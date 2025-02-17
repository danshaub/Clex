Clex
====

**This is a modification of the original lexicon that simply removes all non-ascii characters from the included words. Essentially, any word that has a diacritic is no longer included.**

[clex_lexicon.pl](clex_lexicon.pl) is a large English lexicon derived from COMLEX.
It conforms to the [ACE Lexicon Specification](http://attempto.ifi.uzh.ch/site/docs/ace_lexicon.html)
and can be used as a drop-in replacement for the (small) lexicon file
included in the [APE source distribution](https://github.com/Attempto/APE).

In order to replace the lexicon that is included in the APE source
with this large lexicon go into the root directory of the APE source,
copy the large lexicon over `lexicon/clex_lexicon.pl` and recompile APE,
e.g. by using these commands.

	curl -L https://raw.githubusercontent.com/danshaub/Clex/master/clex_lexicon.pl > prolog/lexicon/clex_lexicon.pl
	make build

Instead of `curl` one can also use `wget` to download the lexicon.

	wget -O - https://raw.githubusercontent.com/danshaub/Clex/master/clex_lexicon.pl > prolog/lexicon/clex_lexicon.pl
