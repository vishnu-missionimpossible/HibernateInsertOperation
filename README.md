# HibernateInsertOperation


HQLInsert operation
---------------------------
It is not possible to insert one record to the database directly using insert
query,becoz linking generators with HQL insert query
is not possible. so we use session.save() method to insert a record.
We can use HQL insert query to insert bulk record into one db table by selecting
them from another db table.

eg: insert into .... values (query is not given)
insert into ... SELECT FROM ...... (given to perform bulk

operation)
insurance policy (table filled with records) ---------->
premium_insurance_policy(new table) where tenure>=25 years
