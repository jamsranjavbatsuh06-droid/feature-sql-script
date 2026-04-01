$source = "C:\ProgramData\MySQL\MySQL Server 8.0\Data\DESKTOP-QA5HAO2.log"
$destination = "C:\audit_logs\DESKTOP-QA5HAO2.log"

 #while($true){
 #   Copy-Item $source -Destination $destination -Force
 #   Start-Sleep-Seconds 3
#}

while ($true) {
    Copy-Item $source -Destination $destination -Force
    Write-Host "Copied at $(Get-Date)" -ForegroundColor Green
    Start-Sleep -Seconds 3
}
[DESKTOP-QA5HAO2.log](https://github.com/user-attachments/files/26394818/DESKTOP-QA5HAO2.log)
C:\Program Files\MySQL\MySQL Server 8.0\bin\mysqld.exe, Version: 8.0.45 (MySQL Community Server - GPL). started with:
TCP Port: 3306, Named Pipe: MySQL
Time                 Id Command    Argument
2026-04-01T00:45:35.831511Z	   10 Query	show variables like 'general_log_file'
2026-04-01T00:45:35.841971Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T00:45:35.846866Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 591
2026-04-01T00:45:35.847609Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 591
2026-04-01T00:46:18.961802Z	   10 Query	select * from sql_invoicig.clients
LIMIT 0, 1000
2026-04-01T00:46:29.858461Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T00:46:29.866224Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T00:46:29.866696Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 595
2026-04-01T00:46:29.866853Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 595
2026-04-01T00:46:29.867249Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T00:51:28.471748Z	   10 Query	insert into sql_invoicing.clients
(client_id, name, address, city, state, phone) values
(6, 'TestClient', '123 Test Street', 'TestCity', 'TC', '999-999-9999')
2026-04-01T00:52:56.751871Z	   10 Query	update sql_invoicing.clients
set city = 'UpdateCity' where name = 'TestClient'
2026-04-01T00:54:07.896592Z	   10 Query	update sql_invoicing.clients
set city = 'UpdateCity' 
where name = 'TestClient'
2026-04-01T00:56:22.830741Z	   10 Query	update sql_invoicing.clients
set city = 'UpdatedCity' 
where name = 'TestClient'
2026-04-01T00:58:33.757859Z	   10 Query	insert into sql_invoicing.clients
(client_id, name, address, city, state, phone) values
(6, 'TestClient', '123 Test Street', 'TestCity', 'TC', '999-999-9999')
2026-04-01T00:58:41.280739Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T00:58:41.287304Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T00:58:41.287938Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 614
2026-04-01T00:58:41.288128Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 614
2026-04-01T00:58:41.288486Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T00:58:47.323120Z	   10 Query	update sql_invoicing.clients
set city = 'UpdatedCity' 
where name = 'TestClient'
2026-04-01T00:58:50.455636Z	   10 Query	update sql_invoicing.clients
set city = 'UpdatedCity' 
where name = 'TestClient'
2026-04-01T00:58:52.759732Z	   10 Query	update sql_invoicing.clients
set city = 'UpdatedCity' 
where name = 'TestClient'
2026-04-01T01:00:54.511544Z	   10 Query	update sql_invoicing.clients
set city = 'UpdatedCity' 
where client_id = 6
2026-04-01T01:01:00.055575Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:01:00.061221Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:01:00.061811Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 629
2026-04-01T01:01:00.061982Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 629
2026-04-01T01:01:00.062402Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T01:02:00.386639Z	   10 Query	delete from sql_invoicing.clients
where name = 'TestClients'
2026-04-01T01:02:22.743101Z	   10 Query	delete from sql_invoicing.clients
where name = 'TestClient'
2026-04-01T01:04:37.127409Z	   10 Query	delete from sql_invoicing.clients
where client_id = 6
2026-04-01T01:05:32.063372Z	   10 Query	show variables like 'general_log_file'
2026-04-01T01:05:32.071201Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:05:32.071735Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 642
2026-04-01T01:05:32.071919Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 642
2026-04-01T01:16:04.270985Z	   10 Query	set global general_log = 'on'
2026-04-01T01:27:36.179609Z	   10 Query	select * from invoices
LIMIT 0, 1000
2026-04-01T01:28:15.881423Z	    9 Query	SHOW DATABASES
2026-04-01T01:28:15.952849Z	    9 Query	SHOW FULL TABLES FROM `sql_inventory`
2026-04-01T01:28:15.954308Z	    9 Query	SHOW PROCEDURE STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:15.955232Z	    9 Query	SHOW FUNCTION STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:15.956201Z	   10 Query	SHOW FULL COLUMNS FROM `sql_inventory`.`products`
2026-04-01T01:28:16.545361Z	    9 Query	SHOW DATABASES
2026-04-01T01:28:16.608527Z	    9 Query	SHOW FULL TABLES FROM `sql_inventory`
2026-04-01T01:28:16.609705Z	    9 Query	SHOW PROCEDURE STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:16.610672Z	    9 Query	SHOW FUNCTION STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:16.611596Z	   10 Query	SHOW FULL COLUMNS FROM `sql_inventory`.`products`
2026-04-01T01:28:17.112608Z	    9 Query	SHOW DATABASES
2026-04-01T01:28:17.154991Z	    9 Query	SHOW FULL TABLES FROM `sql_inventory`
2026-04-01T01:28:17.156141Z	    9 Query	SHOW PROCEDURE STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:17.157125Z	    9 Query	SHOW FUNCTION STATUS WHERE Db='sql_inventory'
2026-04-01T01:28:17.158069Z	   10 Query	SHOW FULL COLUMNS FROM `sql_inventory`.`products`
2026-04-01T01:28:22.216606Z	    9 Query	SHOW FULL TABLES FROM `sql_store`
2026-04-01T01:28:22.218104Z	    9 Query	SHOW PROCEDURE STATUS WHERE Db='sql_store'
2026-04-01T01:28:22.219061Z	    9 Query	SHOW FUNCTION STATUS WHERE Db='sql_store'
2026-04-01T01:28:22.220447Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`customers`
2026-04-01T01:28:22.222240Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`order_item_notes`
2026-04-01T01:28:22.222918Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`order_items`
2026-04-01T01:28:22.223942Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`order_statuses`
2026-04-01T01:28:22.224899Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`orders`
2026-04-01T01:28:22.225663Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`products`
2026-04-01T01:28:22.226243Z	   10 Query	SHOW FULL COLUMNS FROM `sql_store`.`shippers`
2026-04-01T01:28:40.661351Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:28:40.669311Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:28:40.669698Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 674
2026-04-01T01:28:40.669794Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 674
2026-04-01T01:28:40.670123Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T01:29:10.578398Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:29:10.581529Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:29:10.581990Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 677
2026-04-01T01:29:10.582269Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 677
2026-04-01T01:29:10.582995Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T01:32:26.024075Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:32:26.035353Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:32:26.035890Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 680
2026-04-01T01:32:26.036134Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 680
2026-04-01T01:32:26.036546Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T01:33:40.950512Z	   10 Query	delete from sql_invoicing.clients where client_id = 1
2026-04-01T01:38:51.620404Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:38:51.627688Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:38:51.628058Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 687
2026-04-01T01:38:51.628153Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 687
2026-04-01T01:38:51.628502Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T01:39:26.655809Z	   10 Query	delete from sql_invoicing.clients where client_id = 2
2026-04-01T01:39:36.364163Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T01:39:36.370993Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T01:39:36.371378Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 693
2026-04-01T01:39:36.371512Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 693
2026-04-01T01:39:36.371911Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T02:12:16.683276Z	   10 Query	set global general_log = 'on'
2026-04-01T02:12:24.931771Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T02:12:24.939017Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T02:12:24.939580Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 701
2026-04-01T02:12:24.940024Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 701
2026-04-01T02:12:24.940686Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T02:12:37.499315Z	   10 Query	delete from sql_invoicing.clients where client_id = 3
2026-04-01T02:22:12.162228Z	   10 Query	select * from sql_invoicing.clients
LIMIT 0, 1000
2026-04-01T02:22:12.169144Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T02:22:12.169515Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 708
2026-04-01T02:22:12.169630Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 708
2026-04-01T02:22:12.170003Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`clients`
2026-04-01T02:25:28.189486Z	   10 Query	select * from sql_invoicing.payment_methods
LIMIT 0, 1000
2026-04-01T02:25:28.196154Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T02:25:28.196500Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 712
2026-04-01T02:25:28.196605Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 712
2026-04-01T02:25:28.197144Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`payment_methods`
2026-04-01T02:33:16.164510Z	   10 Query	select * from sql_invoicing.payments
LIMIT 0, 1000
2026-04-01T02:33:16.170735Z	    9 Query	SELECT st.* FROM performance_schema.events_statements_current st JOIN performance_schema.threads thr ON thr.thread_id = st.thread_id WHERE thr.processlist_id = 10
2026-04-01T02:33:16.171148Z	    9 Query	SELECT st.* FROM performance_schema.events_stages_history_long st WHERE st.nesting_event_id = 715
2026-04-01T02:33:16.171380Z	    9 Query	SELECT st.* FROM performance_schema.events_waits_history_long st WHERE st.nesting_event_id = 715
2026-04-01T02:33:16.171865Z	    9 Query	SHOW INDEX FROM `sql_invoicing`.`payments`
2026-04-01T02:36:02.326092Z	   10 Query	delete from sql_invoicing.clients
2026-04-01T02:37:53.348103Z	   10 Quit	
2026-04-01T02:37:53.348284Z	    9 Quit	
2026-04-01T02:37:57.033794Z	   11 Connect	root@localhost on  using SSL/TLS
2026-04-01T02:37:57.033873Z	   11 Connect	Access denied for user 'root'@'localhost' (using password: NO)
2026-04-01T02:38:08.890089Z	   12 Connect	root@localhost on  using SSL/TLS
2026-04-01T02:38:08.890302Z	   12 Query	set autocommit=1
2026-04-01T02:38:08.890592Z	   12 Query	SELECT current_user()
2026-04-01T02:38:08.890873Z	   12 Query	SET CHARACTER SET utf8
2026-04-01T02:38:08.891121Z	   12 Query	SET NAMES utf8
2026-04-01T02:38:08.891371Z	   12 Query	SHOW SESSION VARIABLES LIKE 'sql_mode'
2026-04-01T02:38:08.893991Z	   12 Query	SELECT CONNECTION_ID()
2026-04-01T02:38:08.894100Z	   12 Query	show character set where charset = 'utf8mb4'
2026-04-01T02:38:08.894793Z	   12 Query	SET NAMES 'utf8mb4'
2026-04-01T02:38:08.895089Z	   12 Query	SHOW SESSION STATUS LIKE 'Ssl_cipher'
2026-04-01T02:38:08.897117Z	   12 Query	set autocommit=1
2026-04-01T02:38:08.921655Z	   13 Connect	root@localhost on  using SSL/TLS
2026-04-01T02:38:08.921931Z	   13 Query	set autocommit=1
2026-04-01T02:38:08.922073Z	   13 Query	SELECT current_user()
2026-04-01T02:38:08.922319Z	   13 Query	SET CHARACTER SET utf8
2026-04-01T02:38:08.922457Z	   13 Query	SET NAMES utf8
2026-04-01T02:38:08.922526Z	   13 Query	SELECT CONNECTION_ID()
2026-04-01T02:38:08.922758Z	   13 Query	show character set where charset = 'utf8mb4'
2026-04-01T02:38:08.923377Z	   13 Query	SET NAMES 'utf8mb4'
2026-04-01T02:38:08.923650Z	   13 Query	SHOW SESSION STATUS LIKE 'Ssl_cipher'
2026-04-01T02:38:08.924242Z	   13 Query	set autocommit=1
2026-04-01T02:38:08.924379Z	   13 Query	SHOW SESSION VARIABLES LIKE 'sql_mode'
2026-04-01T02:38:08.926051Z	   13 Query	SHOW SESSION VARIABLES LIKE 'version_comment'
2026-04-01T02:38:08.926683Z	   13 Query	SHOW SESSION VARIABLES LIKE 'version'
2026-04-01T02:38:08.927717Z	   13 Query	SELECT current_user()
2026-04-01T02:38:08.927905Z	   13 Query	SHOW SESSION VARIABLES LIKE 'lower_case_table_names'
2026-04-01T02:38:09.069067Z	   13 Query	show engines
2026-04-01T02:38:09.069204Z	   12 Query	SHOW DATABASES
2026-04-01T02:38:09.069339Z	   13 Query	show charset
2026-04-01T02:38:09.070092Z	   13 Query	show collation
2026-04-01T02:38:09.071352Z	   13 Query	show variables
2026-04-01T02:38:09.072519Z	   13 Query	SHOW SESSION VARIABLES LIKE 'version_compile_os'
2026-04-01T02:38:09.073394Z	   13 Query	SHOW SESSION VARIABLES LIKE 'offline_mode'
2026-04-01T02:38:09.092851Z	   13 Query	SHOW SESSION VARIABLES LIKE 'wait_timeout'
2026-04-01T02:38:09.093699Z	   13 Query	SHOW SESSION VARIABLES LIKE 'interactive_timeout'
2026-04-01T02:38:17.553394Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:38:32.657734Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:38:36.080593Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:39:10.008482Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:41:05.929267Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:41:06.184065Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:41:06.568867Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:41:06.905035Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:41:07.401025Z	   13 Query	delete from sql_invoicing.clients
2026-04-01T02:43:21.601164Z	   13 Query	SET FOREIGN_KEY_CHECKS = 0
2026-04-01T02:43:24.369057Z	   13 Query	DELETE FROM sql_invoicing.clients
2026-04-01T02:43:26.616707Z	   13 Query	SET FOREIGN_KEY_CHECKS = 1
2026-04-01T02:51:15.894711Z	   13 Quit	
2026-04-01T02:51:15.894820Z	   12 Quit	
[DESKTOP-QA5HAO2_app.log](https://github.com/user-attachments/files/26394821/DESKTOP-QA5HAO2_app.log)

[siem.py](https://github.com/user-attachments/files/26394822/siem.py)


[1.sql](https://github.com/user-attachments/files/26394824/1.sql)
DROP DATABASE IF EXISTS `sql_invoicing`;
CREATE DATABASE `sql_invoicing`; 
USE `sql_invoicing`;

SET NAMES utf8 ;
SET character_set_client = utf8mb4 ;

CREATE TABLE `payment_methods` (
  `payment_method_id` tinyint(4) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  PRIMARY KEY (`payment_method_id`)
) ENGINE=InnoDB AUTO_INCREMENT=5 DEFAULT CHARSET=utf8mb4;
INSERT INTO `payment_methods` VALUES (1,'Credit Card');
INSERT INTO `payment_methods` VALUES (2,'Cash');
INSERT INTO `payment_methods` VALUES (3,'PayPal');
INSERT INTO `payment_methods` VALUES (4,'Wire Transfer');

CREATE TABLE `clients` (
  `client_id` int(11) NOT NULL,
  `name` varchar(50) NOT NULL,
  `address` varchar(50) NOT NULL,
  `city` varchar(50) NOT NULL,
  `state` char(2) NOT NULL,
  `phone` varchar(50) DEFAULT NULL,
  PRIMARY KEY (`client_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `clients` VALUES (1,'Vinte','3 Nevada Parkway','Syracuse','NY','315-252-7305');
INSERT INTO `clients` VALUES (2,'Myworks','34267 Glendale Parkway','Huntington','WV','304-659-1170');
INSERT INTO `clients` VALUES (3,'Yadel','096 Pawling Parkway','San Francisco','CA','415-144-6037');
INSERT INTO `clients` VALUES (4,'Kwideo','81674 Westerfield Circle','Waco','TX','254-750-0784');
INSERT INTO `clients` VALUES (5,'Topiclounge','0863 Farmco Road','Portland','OR','971-888-9129');

CREATE TABLE `invoices` (
  `invoice_id` int(11) NOT NULL,
  `number` varchar(50) NOT NULL,
  `client_id` int(11) NOT NULL,
  `invoice_total` decimal(9,2) NOT NULL,
  `payment_total` decimal(9,2) NOT NULL DEFAULT '0.00',
  `invoice_date` date NOT NULL,
  `due_date` date NOT NULL,
  `payment_date` date DEFAULT NULL,
  PRIMARY KEY (`invoice_id`),
  KEY `FK_client_id` (`client_id`),
  CONSTRAINT `FK_client_id` FOREIGN KEY (`client_id`) REFERENCES `clients` (`client_id`) ON DELETE RESTRICT ON UPDATE CASCADE
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `invoices` VALUES (1,'91-953-3396',2,101.79,0.00,'2019-03-09','2019-03-29',NULL);
INSERT INTO `invoices` VALUES (2,'03-898-6735',5,175.32,8.18,'2019-06-11','2019-07-01','2019-02-12');
INSERT INTO `invoices` VALUES (3,'20-228-0335',5,147.99,0.00,'2019-07-31','2019-08-20',NULL);
INSERT INTO `invoices` VALUES (4,'56-934-0748',3,152.21,0.00,'2019-03-08','2019-03-28',NULL);
INSERT INTO `invoices` VALUES (5,'87-052-3121',5,169.36,0.00,'2019-07-18','2019-08-07',NULL);
INSERT INTO `invoices` VALUES (6,'75-587-6626',1,157.78,74.55,'2019-01-29','2019-02-18','2019-01-03');
INSERT INTO `invoices` VALUES (7,'68-093-9863',3,133.87,0.00,'2019-09-04','2019-09-24',NULL);
INSERT INTO `invoices` VALUES (8,'78-145-1093',1,189.12,0.00,'2019-05-20','2019-06-09',NULL);
INSERT INTO `invoices` VALUES (9,'77-593-0081',5,172.17,0.00,'2019-07-09','2019-07-29',NULL);
INSERT INTO `invoices` VALUES (10,'48-266-1517',1,159.50,0.00,'2019-06-30','2019-07-20',NULL);
INSERT INTO `invoices` VALUES (11,'20-848-0181',3,126.15,0.03,'2019-01-07','2019-01-27','2019-01-11');
INSERT INTO `invoices` VALUES (13,'41-666-1035',5,135.01,87.44,'2019-06-25','2019-07-15','2019-01-26');
INSERT INTO `invoices` VALUES (15,'55-105-9605',3,167.29,80.31,'2019-11-25','2019-12-15','2019-01-15');
INSERT INTO `invoices` VALUES (16,'10-451-8824',1,162.02,0.00,'2019-03-30','2019-04-19',NULL);
INSERT INTO `invoices` VALUES (17,'33-615-4694',3,126.38,68.10,'2019-07-30','2019-08-19','2019-01-15');
INSERT INTO `invoices` VALUES (18,'52-269-9803',5,180.17,42.77,'2019-05-23','2019-06-12','2019-01-08');
INSERT INTO `invoices` VALUES (19,'83-559-4105',1,134.47,0.00,'2019-11-23','2019-12-13',NULL);

CREATE TABLE `payments` (
  `payment_id` int(11) NOT NULL AUTO_INCREMENT,
  `client_id` int(11) NOT NULL,
  `invoice_id` int(11) NOT NULL,
  `date` date NOT NULL,
  `amount` decimal(9,2) NOT NULL,
  `payment_method` tinyint(4) NOT NULL,
  PRIMARY KEY (`payment_id`),
  KEY `fk_client_id_idx` (`client_id`),
  KEY `fk_invoice_id_idx` (`invoice_id`),
  KEY `fk_payment_payment_method_idx` (`payment_method`),
  CONSTRAINT `fk_payment_client` FOREIGN KEY (`client_id`) REFERENCES `clients` (`client_id`) ON UPDATE CASCADE,
  CONSTRAINT `fk_payment_invoice` FOREIGN KEY (`invoice_id`) REFERENCES `invoices` (`invoice_id`) ON UPDATE CASCADE,
  CONSTRAINT `fk_payment_payment_method` FOREIGN KEY (`payment_method`) REFERENCES `payment_methods` (`payment_method_id`)
) ENGINE=InnoDB AUTO_INCREMENT=9 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `payments` VALUES (1,5,2,'2019-02-12',8.18,1);
INSERT INTO `payments` VALUES (2,1,6,'2019-01-03',74.55,1);
INSERT INTO `payments` VALUES (3,3,11,'2019-01-11',0.03,1);
INSERT INTO `payments` VALUES (4,5,13,'2019-01-26',87.44,1);
INSERT INTO `payments` VALUES (5,3,15,'2019-01-15',80.31,1);
INSERT INTO `payments` VALUES (6,3,17,'2019-01-15',68.10,1);
INSERT INTO `payments` VALUES (7,5,18,'2019-01-08',32.77,1);
INSERT INTO `payments` VALUES (8,5,18,'2019-01-08',10.00,2);


DROP DATABASE IF EXISTS `sql_store`;
CREATE DATABASE `sql_store`;
USE `sql_store`;

CREATE TABLE `products` (
  `product_id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  `quantity_in_stock` int(11) NOT NULL,
  `unit_price` decimal(4,2) NOT NULL,
  PRIMARY KEY (`product_id`)
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `products` VALUES (1,'Foam Dinner Plate',70,1.21);
INSERT INTO `products` VALUES (2,'Pork - Bacon,back Peameal',49,4.65);
INSERT INTO `products` VALUES (3,'Lettuce - Romaine, Heart',38,3.35);
INSERT INTO `products` VALUES (4,'Brocolinni - Gaylan, Chinese',90,4.53);
INSERT INTO `products` VALUES (5,'Sauce - Ranch Dressing',94,1.63);
INSERT INTO `products` VALUES (6,'Petit Baguette',14,2.39);
INSERT INTO `products` VALUES (7,'Sweet Pea Sprouts',98,3.29);
INSERT INTO `products` VALUES (8,'Island Oasis - Raspberry',26,0.74);
INSERT INTO `products` VALUES (9,'Longan',67,2.26);
INSERT INTO `products` VALUES (10,'Broom - Push',6,1.09);


CREATE TABLE `shippers` (
  `shipper_id` smallint(6) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  PRIMARY KEY (`shipper_id`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `shippers` VALUES (1,'Hettinger LLC');
INSERT INTO `shippers` VALUES (2,'Schinner-Predovic');
INSERT INTO `shippers` VALUES (3,'Satterfield LLC');
INSERT INTO `shippers` VALUES (4,'Mraz, Renner and Nolan');
INSERT INTO `shippers` VALUES (5,'Waters, Mayert and Prohaska');


CREATE TABLE `customers` (
  `customer_id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(50) NOT NULL,
  `last_name` varchar(50) NOT NULL,
  `birth_date` date DEFAULT NULL,
  `phone` varchar(50) DEFAULT NULL,
  `address` varchar(50) NOT NULL,
  `city` varchar(50) NOT NULL,
  `state` char(2) NOT NULL,
  `points` int(11) NOT NULL DEFAULT '0',
  PRIMARY KEY (`customer_id`)
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `customers` VALUES (1,'Babara','MacCaffrey','1986-03-28','781-932-9754','0 Sage Terrace','Waltham','MA',2273);
INSERT INTO `customers` VALUES (2,'Ines','Brushfield','1986-04-13','804-427-9456','14187 Commercial Trail','Hampton','VA',947);
INSERT INTO `customers` VALUES (3,'Freddi','Boagey','1985-02-07','719-724-7869','251 Springs Junction','Colorado Springs','CO',2967);
INSERT INTO `customers` VALUES (4,'Ambur','Roseburgh','1974-04-14','407-231-8017','30 Arapahoe Terrace','Orlando','FL',457);
INSERT INTO `customers` VALUES (5,'Clemmie','Betchley','1973-11-07',NULL,'5 Spohn Circle','Arlington','TX',3675);
INSERT INTO `customers` VALUES (6,'Elka','Twiddell','1991-09-04','312-480-8498','7 Manley Drive','Chicago','IL',3073);
INSERT INTO `customers` VALUES (7,'Ilene','Dowson','1964-08-30','615-641-4759','50 Lillian Crossing','Nashville','TN',1672);
INSERT INTO `customers` VALUES (8,'Thacher','Naseby','1993-07-17','941-527-3977','538 Mosinee Center','Sarasota','FL',205);
INSERT INTO `customers` VALUES (9,'Romola','Rumgay','1992-05-23','559-181-3744','3520 Ohio Trail','Visalia','CA',1486);
INSERT INTO `customers` VALUES (10,'Levy','Mynett','1969-10-13','404-246-3370','68 Lawn Avenue','Atlanta','GA',796);


CREATE TABLE `order_statuses` (
  `order_status_id` tinyint(4) NOT NULL,
  `name` varchar(50) NOT NULL,
  PRIMARY KEY (`order_status_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `order_statuses` VALUES (1,'Processed');
INSERT INTO `order_statuses` VALUES (2,'Shipped');
INSERT INTO `order_statuses` VALUES (3,'Delivered');


CREATE TABLE `orders` (
  `order_id` int(11) NOT NULL AUTO_INCREMENT,
  `customer_id` int(11) NOT NULL,
  `order_date` date NOT NULL,
  `status` tinyint(4) NOT NULL DEFAULT '1',
  `comments` varchar(2000) DEFAULT NULL,
  `shipped_date` date DEFAULT NULL,
  `shipper_id` smallint(6) DEFAULT NULL,
  PRIMARY KEY (`order_id`),
  KEY `fk_orders_customers_idx` (`customer_id`),
  KEY `fk_orders_shippers_idx` (`shipper_id`),
  KEY `fk_orders_order_statuses_idx` (`status`),
  CONSTRAINT `fk_orders_customers` FOREIGN KEY (`customer_id`) REFERENCES `customers` (`customer_id`) ON UPDATE CASCADE,
  CONSTRAINT `fk_orders_order_statuses` FOREIGN KEY (`status`) REFERENCES `order_statuses` (`order_status_id`) ON UPDATE CASCADE,
  CONSTRAINT `fk_orders_shippers` FOREIGN KEY (`shipper_id`) REFERENCES `shippers` (`shipper_id`) ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `orders` VALUES (1,6,'2019-01-30',1,NULL,NULL,NULL);
INSERT INTO `orders` VALUES (2,7,'2018-08-02',2,NULL,'2018-08-03',4);
INSERT INTO `orders` VALUES (3,8,'2017-12-01',1,NULL,NULL,NULL);
INSERT INTO `orders` VALUES (4,2,'2017-01-22',1,NULL,NULL,NULL);
INSERT INTO `orders` VALUES (5,5,'2017-08-25',2,'','2017-08-26',3);
INSERT INTO `orders` VALUES (6,10,'2018-11-18',1,'Aliquam erat volutpat. In congue.',NULL,NULL);
INSERT INTO `orders` VALUES (7,2,'2018-09-22',2,NULL,'2018-09-23',4);
INSERT INTO `orders` VALUES (8,5,'2018-06-08',1,'Mauris enim leo, rhoncus sed, vestibulum sit amet, cursus id, turpis.',NULL,NULL);
INSERT INTO `orders` VALUES (9,10,'2017-07-05',2,'Nulla mollis molestie lorem. Quisque ut erat.','2017-07-06',1);
INSERT INTO `orders` VALUES (10,6,'2018-04-22',2,NULL,'2018-04-23',2);


CREATE TABLE `order_items` (
  `order_id` int(11) NOT NULL AUTO_INCREMENT,
  `product_id` int(11) NOT NULL,
  `quantity` int(11) NOT NULL,
  `unit_price` decimal(4,2) NOT NULL,
  PRIMARY KEY (`order_id`,`product_id`),
  KEY `fk_order_items_products_idx` (`product_id`),
  CONSTRAINT `fk_order_items_orders` FOREIGN KEY (`order_id`) REFERENCES `orders` (`order_id`) ON UPDATE CASCADE,
  CONSTRAINT `fk_order_items_products` FOREIGN KEY (`product_id`) REFERENCES `products` (`product_id`) ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `order_items` VALUES (1,4,4,3.74);
INSERT INTO `order_items` VALUES (2,1,2,9.10);
INSERT INTO `order_items` VALUES (2,4,4,1.66);
INSERT INTO `order_items` VALUES (2,6,2,2.94);
INSERT INTO `order_items` VALUES (3,3,10,9.12);
INSERT INTO `order_items` VALUES (4,3,7,6.99);
INSERT INTO `order_items` VALUES (4,10,7,6.40);
INSERT INTO `order_items` VALUES (5,2,3,9.89);
INSERT INTO `order_items` VALUES (6,1,4,8.65);
INSERT INTO `order_items` VALUES (6,2,4,3.28);
INSERT INTO `order_items` VALUES (6,3,4,7.46);
INSERT INTO `order_items` VALUES (6,5,1,3.45);
INSERT INTO `order_items` VALUES (7,3,7,9.17);
INSERT INTO `order_items` VALUES (8,5,2,6.94);
INSERT INTO `order_items` VALUES (8,8,2,8.59);
INSERT INTO `order_items` VALUES (9,6,5,7.28);
INSERT INTO `order_items` VALUES (10,1,10,6.01);
INSERT INTO `order_items` VALUES (10,9,9,4.28);

CREATE TABLE `sql_store`.`order_item_notes` (
  `note_id` INT NOT NULL,
  `order_Id` INT NOT NULL,
  `product_id` INT NOT NULL,
  `note` VARCHAR(255) NOT NULL,
  PRIMARY KEY (`note_id`));

INSERT INTO `order_item_notes` (`note_id`, `order_Id`, `product_id`, `note`) VALUES ('1', '1', '2', 'first note');
INSERT INTO `order_item_notes` (`note_id`, `order_Id`, `product_id`, `note`) VALUES ('2', '1', '2', 'second note');


DROP DATABASE IF EXISTS `sql_hr`;
CREATE DATABASE `sql_hr`;
USE `sql_hr`;


CREATE TABLE `offices` (
  `office_id` int(11) NOT NULL,
  `address` varchar(50) NOT NULL,
  `city` varchar(50) NOT NULL,
  `state` varchar(50) NOT NULL,
  PRIMARY KEY (`office_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `offices` VALUES (1,'03 Reinke Trail','Cincinnati','OH');
INSERT INTO `offices` VALUES (2,'5507 Becker Terrace','New York City','NY');
INSERT INTO `offices` VALUES (3,'54 Northland Court','Richmond','VA');
INSERT INTO `offices` VALUES (4,'08 South Crossing','Cincinnati','OH');
INSERT INTO `offices` VALUES (5,'553 Maple Drive','Minneapolis','MN');
INSERT INTO `offices` VALUES (6,'23 North Plaza','Aurora','CO');
INSERT INTO `offices` VALUES (7,'9658 Wayridge Court','Boise','ID');
INSERT INTO `offices` VALUES (8,'9 Grayhawk Trail','New York City','NY');
INSERT INTO `offices` VALUES (9,'16862 Westend Hill','Knoxville','TN');
INSERT INTO `offices` VALUES (10,'4 Bluestem Parkway','Savannah','GA');



CREATE TABLE `employees` (
  `employee_id` int(11) NOT NULL,
  `first_name` varchar(50) NOT NULL,
  `last_name` varchar(50) NOT NULL,
  `job_title` varchar(50) NOT NULL,
  `salary` int(11) NOT NULL,
  `reports_to` int(11) DEFAULT NULL,
  `office_id` int(11) NOT NULL,
  PRIMARY KEY (`employee_id`),
  KEY `fk_employees_offices_idx` (`office_id`),
  KEY `fk_employees_employees_idx` (`reports_to`),
  CONSTRAINT `fk_employees_managers` FOREIGN KEY (`reports_to`) REFERENCES `employees` (`employee_id`),
  CONSTRAINT `fk_employees_offices` FOREIGN KEY (`office_id`) REFERENCES `offices` (`office_id`) ON UPDATE CASCADE
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `employees` VALUES (37270,'Yovonnda','Magrannell','Executive Secretary',63996,NULL,10);
INSERT INTO `employees` VALUES (33391,'D\'arcy','Nortunen','Account Executive',62871,37270,1);
INSERT INTO `employees` VALUES (37851,'Sayer','Matterson','Statistician III',98926,37270,1);
INSERT INTO `employees` VALUES (40448,'Mindy','Crissil','Staff Scientist',94860,37270,1);
INSERT INTO `employees` VALUES (56274,'Keriann','Alloisi','VP Marketing',110150,37270,1);
INSERT INTO `employees` VALUES (63196,'Alaster','Scutchin','Assistant Professor',32179,37270,2);
INSERT INTO `employees` VALUES (67009,'North','de Clerc','VP Product Management',114257,37270,2);
INSERT INTO `employees` VALUES (67370,'Elladine','Rising','Social Worker',96767,37270,2);
INSERT INTO `employees` VALUES (68249,'Nisse','Voysey','Financial Advisor',52832,37270,2);
INSERT INTO `employees` VALUES (72540,'Guthrey','Iacopetti','Office Assistant I',117690,37270,3);
INSERT INTO `employees` VALUES (72913,'Kass','Hefferan','Computer Systems Analyst IV',96401,37270,3);
INSERT INTO `employees` VALUES (75900,'Virge','Goodrum','Information Systems Manager',54578,37270,3);
INSERT INTO `employees` VALUES (76196,'Mirilla','Janowski','Cost Accountant',119241,37270,3);
INSERT INTO `employees` VALUES (80529,'Lynde','Aronson','Junior Executive',77182,37270,4);
INSERT INTO `employees` VALUES (80679,'Mildrid','Sokale','Geologist II',67987,37270,4);
INSERT INTO `employees` VALUES (84791,'Hazel','Tarbert','General Manager',93760,37270,4);
INSERT INTO `employees` VALUES (95213,'Cole','Kesterton','Pharmacist',86119,37270,4);
INSERT INTO `employees` VALUES (96513,'Theresa','Binney','Food Chemist',47354,37270,5);
INSERT INTO `employees` VALUES (98374,'Estrellita','Daleman','Staff Accountant IV',70187,37270,5);
INSERT INTO `employees` VALUES (115357,'Ivy','Fearey','Structural Engineer',92710,37270,5);


DROP DATABASE IF EXISTS `sql_inventory`;
CREATE DATABASE `sql_inventory`;
USE `sql_inventory`;


CREATE TABLE `products` (
  `product_id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  `quantity_in_stock` int(11) NOT NULL,
  `unit_price` decimal(4,2) NOT NULL,
  PRIMARY KEY (`product_id`)
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4  ;
INSERT INTO `products` VALUES (1,'Foam Dinner Plate',70,1.21);
INSERT INTO `products` VALUES (2,'Pork - Bacon,back Peameal',49,4.65);
INSERT INTO `products` VALUES (3,'Lettuce - Romaine, Heart',38,3.35);
INSERT INTO `products` VALUES (4,'Brocolinni - Gaylan, Chinese',90,4.53);
INSERT INTO `products` VALUES (5,'Sauce - Ranch Dressing',94,1.63);
INSERT INTO `products` VALUES (6,'Petit Baguette',14,2.39);
INSERT INTO `products` VALUES (7,'Sweet Pea Sprouts',98,3.29);
INSERT INTO `products` VALUES (8,'Island Oasis - Raspberry',26,0.74);
INSERT INTO `products` VALUES (9,'Longan',67,2.26);
INSERT INTO `products` VALUES (10,'Broom - Push',6,1.09);
-- -------------------------------------------------
-- 1
set global general_log = 'on';
-- 2
show variables like 'general_log_file';
-- 3
select * from sql_invoicing.clients;
-- 4
insert into sql_invoicing.clients
(client_id, name, address, city, state, phone) values
(6, 'TestClient', '123 Test Street', 'TestCity', 'TC', '999-999-9999');
-- 5
update sql_invoicing.clients
set city = 'UpdatedCity' 
where client_id = 6; 
-- 6
delete from sql_invoicing.clients
where client_id = 6; 
-- 7
show variables like 'general_log_file';
-- 8
set global general_log = 'on';
-- 9
select * from sql_invoicing.clients;
-- 10
delete from sql_invoicing.clients where client_id = 3;
-- 11
select * from sql_invoicing.payment_methods;
-- 12
select * from sql_invoicing.payments;
-- 13

delete from sql_invoicing.clients;


[audit_logs.zip](https://github.com/user-attachments/files/26394828/audit_logs.zip)
<img width="1919" height="990" alt="ss1" src="https://github.com/user-attachments/assets/79c0cb57-b8a3-4dc1-8bb5-4693649b507c" />
<img width="1919" height="993" alt="ss2" src="https://github.com/user-attachments/assets/e093b372-138f-44d1-9147-bad83773eff8" />
<img width="1909" height="981" alt="ss3" src="https://github.com/user-attachments/assets/f6238a52-0cc9-4fbc-8b32-511ea303eab5" />
<img width="1914" height="982" alt="ss4" src="https://github.com/user-attachments/assets/da40a441-571f-4489-a195-47ce0c4b764d" />
<img width="1859" height="985" alt="ss5" src="https://github.com/user-attachments/assets/96ea5981-40c9-42ea-8fba-0e86592030a1" />
<img width="1176" height="989" alt="ss6" src="https://github.com/user-attachments/assets/9277fe38-2aa4-48f3-aa5a-869a4c351545" />
