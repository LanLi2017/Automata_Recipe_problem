# Automata_Recipe_problem
python 3.6
Use case:  How to preserve data lineage by monitoring foreign keys between linked tables 

When integrating tables R1, …, Rn from multiple sources, the relationships (primary keys and foreign keys)
are hidden (i.e., not visible / not accessible / not known)  in OpenRefine (OR).

In this way, ICs (integration constraints) may be broken because of the manipulations working on the keys through OR: each table Ri might be “cleaned” independently, resulting in different changes, e.g., in parent-child linked tables. For example a foreign key FK of a child table Rc might reference the primary key PK of the parent table Rp:

 Rc.FK → Rp.PK 

Now if Rc and Rp are cleaned separately, the links between FKs and PKs might be lost / broken due to different cleaning operations applied to them.

##
the output file will present the percentage of the matching after data cleaning
Research Problem:
If the dataset includes multiple tables with foreign keys, and users use OpenRefine to do data cleaning with these tables. 
The foreign keys may get broken because of different manipulations on them. 

