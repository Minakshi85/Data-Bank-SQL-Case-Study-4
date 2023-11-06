# Data-Bank-SQL-Case-Study-4


SELECT region_name , COUNT(node_id) AS "Nodes"
FROM data_bank.customer_nodes c
LEFT JOIN data_bank.regions r
ON r.region_id = c.region_id
GROUP BY region_name;
