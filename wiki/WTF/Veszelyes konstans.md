---
creationDate        : 2008-11-02 20:22:35 +0100 
author              : zmb 
title               : WTF/Veszelyes konstans 
name                : WTF/Veszelyes konstans 
layout              : wiki 
path                : WTF/Veszelyes konstans 
date                : 2008-11-02 20:22:35 +0100 
version             : 1 
creator             : zmb 
---
Sokszor elofordul, hogy bizonyos ertekeket konstansokba rakunk, es azokra hivatkozunk. A kovetkezo kis kodreszletben valamiert a fejleszo ugy gondolta, hogy enum segitsegevel jobban megoldhato a problema, mint egyszeru konstanssal.

```
protected int pageLength = PAGE_LENGTH.LENGTH_10.getPageLength();

public static enum PAGE_LENGTH {
	LENGTH_10 {
		public int getPageLength() {
			return 10;
		}

	},
	LENGTH_25 {
		public int getPageLength() {
			return 25;
		}
	},
	LENGTH_50 {
		public int getPageLength() {
			return 50;
		}
	};

	public abstract int getPageLength();
}
```
