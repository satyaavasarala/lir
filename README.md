LIR (Lucene Index Reader)
=========================

`lir` is a Lucene Index reading utility. Right now it can do two things. One, it can read through all the documents available in a index directory and print them out. Secondly, it can search through the index for a field name and value combination, specified by the user,  and retrive all the documents that contain the combination. 

Setup
=====
Clone the repo to your workstation

	git clone https://github.com/satyaavasarala/lir

Set the LIR_HOME in ~/.profile if on Linux or ENV variables if on Windows

	export LIR_HOME=<<your clone location>>

For access to 'lir' from anywhere on your workstation add the following to the PATH

	export PATH="$LIR_HOME/bin:$PATH"


Usage
=====
To list all the documents available in the Lucene Index

	lir -i /Users/satya.avasarala/lucene-data/ -listall

To search for a specific field name and value across all the documents

	lir -i /Users/satya.avasarala/lucene-data/ -search username,john
