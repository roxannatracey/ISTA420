.headers on

--name: cars exercises
--script: cars.sql
--date: January 14, 2020

drop table if exists cars;

create table cars (
	ID integer primary key,
	model text,
	make text,
	doors integer,
	color text
);
insert into cars values (1, 'audi', 'r8', 2, 'black');
insert into cars values (2, 'BMW', 'm5', 4, 'blue');
insert into cars values (3, 'porsche', '718', 2, 'white');
insert into cars values (4, 'nissan', 'gtr', 2, 'yellow');
insert into cars values (5, 'audi', 's6', 4, 'red');

select * from cars;
ID|model|make|doors|color
1|audi|r8|2|black
2|BMW|m5|4|blue
3|porsche|718|2|white
4|nissan|gtr|2|yellow
5|audi|s6|4|red
