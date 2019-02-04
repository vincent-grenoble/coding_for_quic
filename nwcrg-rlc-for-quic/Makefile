# initialize the NAME_BASE variable with the file name without any extension
NAME_BASE=draft-roca-nwcrg-rlc-fec-scheme-for-quic-01
XML=${NAME_BASE}.xml
TXT=${NAME_BASE}.txt
HTML=${NAME_BASE}.html

all:
	xml2rfc --text ${XML}
	xml2rfc --html ${XML}


# specify which version to diff with below
PREV_VERSION=draft-roca-nwcrg-rlc-fec-scheme-for-quic-00.txt
diff:
	rfcdiff.sh ${PREV_VERSION} ${TXT}


clean:
	rm ${TXT}
	rm ${HTML}
