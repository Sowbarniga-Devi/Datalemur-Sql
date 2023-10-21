# Datalemur-Sql

**# Facebook - Page With No Likes**
Assume you're given two tables containing data about Facebook Pages and their respective likes (as in "Like a Facebook Page").

Write a query to return the IDs of the Facebook pages that have zero likes. The output should be sorted in ascending order based on the page IDs.

SELECT A.page_id
FROM pages A
LEFT JOIN page_likes B
ON A.page_id = B.page_id
WHERE B.liked_date is NULL
ORDER BY 1 ASC

page_id
20701
