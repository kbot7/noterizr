# Developer Log
Instructions: Start each log with ISO8601 date time on a new line with content in line below.


2024-08-18 00:26
A note is a document. Therefore, I should approach this as a document database problem. 

Consider using actual files in directories. Consider pros and cons.
Also consider a file-based database, which would be better for encryption.
Maybe just use off-the-shelf file-based document DBs. Mongo supports that.

LiteDB appears to fit my desired criteria:
https://www.litedb.org/
"LiteDB is a serverless database delivered in a single small DLL (< 450kb) fully written in .NET C# managed code (compatible with .NET 4.5 and NETStandard 2.0)."

https://www.litedb.org/docs/encryption/
"LiteDB uses salted AES (as defined by RFC 2898) as its encryption. This is implemented by the Rfc2898DeriveBytes class."

>> LiteDBs encryption could be utilized for global DB encryption. Encrypting each note separately could and should also be done. 


Question for self:
- Can I utilize hardware keys and/or PassKey infrastructure for encryption? Perhaps for viewing?
- Can client devices directly access hardware keys?

Ideally, the digital journal is only available when physical hardware key is plugged in.



