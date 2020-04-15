DB uses three tables "Order", "Tourist", "Equipment"

CREATE DATABASE lab2_prev_semestr;
use lab2_prev_semestr;

create table `Order`
(
	id long auto_increment,
	touristId long not null,
	equipmentId int not null
	constraint Order_pk
		primary key (id)
);

create table Tourist
(
	id int auto_increment,
	name varchar(50) not null,
	email varchar(50) not null,
	constraint Tourist_pk
		primary key (id)
);

create table Equipment
(
	id int auto_increment,
	name varchar(50) not null,
	price float not null,
	type varchar(20) null,
	constraint Equipment_pk
		primary key (id)
);
