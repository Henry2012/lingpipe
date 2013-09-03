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
* Reference
	* http://tech.groups.yahoo.com/group/LingPipe/message/205