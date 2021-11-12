"# TSQL-IDENTITY_INSERT-" 

SET IDENTITY_INSERT db.dbo.umStatus ON;
insert into db.dbo.tbl   ( fq, fe, fg ) 
(SELECT  fq, fe, fg FROM db_sandbox.dbo.tbl);
SET IDENTITY_INSERT db.dbo.tbl OFF;