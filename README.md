# exp9dbms
CREATE DEFINER=`root`@`localhost` PROCEDURE `proc1`()
BEGIN
declare name varchar(20);
declare str varchar(20);
set name='sara';
set str=concat('hello ',name);
select str;
END
CREATE DEFINER=`root`@`localhost` PROCEDURE `addition`()
BEGIN
declare a,b,c int(4);
set a=20,b=30;
set c=a+b;
select c;
END
BEGIN
declare
n int(4);
declare fac,i int(4);
 
set i=1,n=4,fac=1;
while(i<=n) do
set fac=fac*i;
set i=i+1;
end while;
select fac;
END
