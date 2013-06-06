---
creationDate        : 2005-08-02 12:16:04 +0200 
author              : admin 
title               : WTF/BEGIN TRANSACTION 
name                : WTF/BEGIN TRANSACTION 
layout              : wiki 
path                : WTF/BEGIN TRANSACTION 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : suhaig 
---
Szükséges ehhez bármiféle megjegyzés?

```
public int beginTransaction() throws SpecificException
{
	try
	{
		if (DB_TYPE.equals(DBTYPE_SQLSERVER))
			executeUpdate("BEGIN TRANSACTION", null);
		else
			return 0;
	}
	catch (Exception ex)
	{
		throw new SpecificException(SpecificException.ERROR_IN_DBCONNECTION);
	
	}
}
```
