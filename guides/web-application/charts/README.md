---
description: This chapter is dedicated to describing how to create charts in footprints
---

# Charts

Although the volumes handled by Footprint are enormous and require a very sophisticated technical solution to ensure sufficient performance in processing queries, Footprint has a relational database under the hood. Data retrieval from the relational database is done via SQL. Thus, the process of forming a data query is as follows:

1. User creates a query in UI
2. Query translated to SQL
3. SQL query is executed on database

Footprint is a easy-to-use analytics tool that the user can work with without knowledge of SQL, programming languages and other technical aspects - see [get-started-with-creating-a-chart.md](get-started-with-creating-a-chart.md "mention"). Nevertheless, if you prefer to keep everything as code; want to create more complex queries; want to run query optimisations or for any other reason you may skip the **point 1** in the list above and create a SQL query straight away - see [sql](sql/ "mention").
