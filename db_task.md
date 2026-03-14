Первое задание
1. \d+ "Couriers"
2. \d+ "Orders"
3. SELECT c."login", COUNT(o."id") AS orders_in_delivery FROM "Couriers" c JOIN "Orders" o ON o."courierId" = c."id" WHERE o."inDelivery" = true GROUP BY c."login";
Второе задание 
SELECT "track", CASE WHEN "finished" = true THEN 2 WHEN "cancelled" = true THEN -1 WHEN "inDelivery" = true THEN 1 ELSE 0 END AS status FROM "Orders";