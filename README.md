# CalculateAge
===============
Calculate age in php by age calculator function.
Auwal
Nazief
#### Usage
Just call function ageCalculator(Date, format), Date parameter must be DateTime and possible formats are mentioned below.

<strong>Examples;</strong>

ageCalculator( new DateTime('1982-07-24') ); //33 years, 1 month and 9 days

If you are using laravel then it is more easy with Carbon like ageCalculator( new Carbon('1982-07-24') );

ageCalculator( new DateTime('1982-07-24'), 'd' ); //1201

ageCalculator( new DateTime('1982-07-24'), 'D' ); //1201 days

ageCalculator( new DateTime('1982-07-24'), '%m' ); //1

ageCalculator( new DateTime('1982-07-24'), '%M' ); //1 month

ageCalculator( new DateTime('1982-07-24'), '%y y, %m m and %d days old' ); //33 y, 1 m and 9 days old

ageCalculator( new DateTime('1982-07-24'), '%Y, %M and %D old' ); //33 years, 1 month and 9 days old



#### Possible Formats
d -- It returns total number of days in numeric.

m -- It returns total number of months in numeric.

y -- It returns total number of years in numeric.

D -- It returns in string with total number of days like 400 days or 1 day.

M -- It returns in string with total number of months like 397 months or 1 month.

Y -- It returns in string with total number of years like 33 years or 1 year

GET RETURN WITH CUSTOM FORMAT, THIS WILL RETURN FROM '33 years 1 month 19 days'. FOR EXAMPLE, IF YOU WANT NUMBER OF DAYS THEN IT WILL ONLY GET NUMBER OF DAYS FROM MENTIONED EXAMPLE INSTEAD TOTAL NUMBER OF DAYS COUNT FROM DAY YOU BORN.

%d -- It returns number of days but not same as above d. It returns number of days from 33 years 1 month 19 days.

%m -- It returns number of months, maximum month is 11.

%y -- It returns number of years, how old you are.

%D -- It returns with string, don't worry about singular and plural.

%M -- It returns with string.

%Y -- It returns with string.
