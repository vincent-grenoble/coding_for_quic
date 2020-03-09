# initialize the NAME_BASE variable with the file name without any extension
NAME_BASE=draft-swett-nwcrg-coding-for-quic-04
XML=${NAME_BASE}.xml
TXT=${NAME_BASE}.txt
HTML=${NAME_BASE}.html

# Removed:html output is broken (bugs)...	xml2rfc --html ${XML}	
all:
	xml2rfc --text ${XML}


# specify which version to diff with below
PREV_VERSION=archives/draft-swett-nwcrg-coding-for-quic-03.txt

diff:
	rfcdiff.sh ${PREV_VERSION} ${TXT}


clean:
	rm ${TXT}
	rm ${HTML}
