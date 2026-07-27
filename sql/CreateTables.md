USE umar\_DWH

GO

CREATE SCHEMA gold



\----------------------------------------



### **--CTAS enr\_customers**

\--------------------------

create table umar\_DWH.gold.cur\_customers

AS

SELECT \* from Silver\_Lakehouse.dbo.customers\_enr





### \--CTAS enr\_orderitems

\--------------------------

create table umar\_DWH.gold.cur\_orderitems

AS

SELECT \* from Silver\_Lakehouse.dbo.enr\_orderitems





### \--CTAS enr\_orders

\--------------------------

create table umar\_DWH.gold.cur\_orders

AS

SELECT \* from Silver\_Lakehouse.dbo.enr\_orders





### \--CTAS enr\_payments

\--------------------------

create table umar\_DWH.gold.cur\_payments

AS

SELECT \* from Silver\_Lakehouse.dbo.enr\_payments





### \--CTAS enr\_products

\--------------------------

create table umar\_DWH.gold.cur\_products

AS

SELECT \* from Silver\_Lakehouse.dbo.enr\_products



### \--CTAS enr\_reviews

\--------------------------

create table umar\_DWH.gold.cur\_reviews

AS

SELECT \* from Silver\_Lakehouse.dbo.enr\_reviews





