LingPipe
===
* character-based outperformed token-based
	* character-based: predict the next character given the previous N characters
	* token-based: predict the next word given the previous M words
	* N can be much bigger than M for models of the same size on disk
	* why?
		* no tokenization issues
		* more robust to alternative spellings, morphology, etc
			* trained on "language" matches "languages"
			* trained on "p-53" might match "p53" pretty well
			* the tokens "p" and "53" don't match the token "p53"
* Can't run through the demo in [Character LM Tutorial](http://alias-i.com/lingpipe/demos/tutorial/lm/read-me.html)	
	* in the tutorial, ant is used, but i turned to configure arguments in Run Configurations of eclipse
	* The output always throw _Exception in thread "main" java.lang.ClassNotFoundException: com.aliasi.corpus.parsers.MedlineTextParser_ like in [the link](http://groups.yahoo.com/neo/groups/LingPipe/conversations/topics/1030)

* Reference
	* http://tech.groups.yahoo.com/group/LingPipe/message/205