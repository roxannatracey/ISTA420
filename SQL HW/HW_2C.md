### Roxanna Barahona
### SQL HW 2C

1. List the date/time types in T-SQL.
The date/time types are as follows.
- DATETIME
- SMALLDATETIME
- DATE
- TIME
- DATETIME2
- DATETIMEOFFSET

2. How do you express a date/time literal in T-SQL?
- You can specify a literal of a different type that can be converted, explicitly, or implicitly - to a date and time data type.

3. What is the setting DATEFORMAT used for?
- DATEFORMAT which determines how SQL server interprets the literals you enter when they are converted from a character-string type to a date and time type. The DATEFORMAT setting is expressed as a combination of the characters d, m, and y.

4. Written a T-SQL snippet changing the date format to German. Read the documentation on how to do
this.
- The DATEFORMAT setting is expressed as a combination of the characters d, m, and y. For example, the US English language setting sets the DATEFORMAT to m, d, y, whereas the British language setting sets the DATEFORMAT to d, m, y.

5. What is the difference between CAST(), CONVERT(), and PARSE()?
- The CAST, CONVERT, and PARSE functions are used to convert an input value to some target
type.

- cast():  used to convert a data type variable or data from one data type to another data type. The Cast() function provides a data type to a dynamic parameter (?) or a NULL value.
- convert():  converts an expression from one datatype to another datatype
- parse (): used to convert the String data to the requested data type and returns the result as an expression.

6. What function returns the current date? This is very useful in a table that maintains a log of events, such as user logins.
- SYSDATETIME
7. How do you add one day to the current date? Add one week? Add one month? Add one year?
-
8. Write a SQL snippet to return the number of years between your birth date and today’s date.
- select julianday('now') - julianday('1994-04-30');

9. How do you check a string literal to see if it represents a valid date?
- SQL Server recognizes the literal ‘20160212’ as a character-string literal and not as a date
and time literal, but because the expression involves operands of two different types, one
operand needs to be implicitly converted to the other ’s type.
- ISDATE()

10. What does EOMONTH() do? Give an example of why this might be very useful.
- IT accepts an input date and time value and returns the respective end-of-month date as a DATE typed value.

11. Payments are due exactly 30 days from the date of the last function. Write a select query that calculates
the date of the next payment. Pretend we want to update a column in a database that contains the
date of the next payment. We will do this when we write UPDATE queries.
- DATEADD(month, 1, 'now')

12. Suppose your son or daughter wants to run a query every day that tells them the number of days until
their 16th birthday. Write a select query that does this.
- DATEDIFF(datepart, startdate, enddate);
