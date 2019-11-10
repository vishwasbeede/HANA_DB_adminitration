HANA administration which requires access to system information. HANA studio provides inforamtion using SYS tables.
Below tables provides information to HANA studio. It is possible for further troubleshooting on HANA DB with these tables.


Syntyax:
SELECT TABLE_NAME FROM SYS.M_TABLES
SELECT * FROM SYS.M_LICENSES
....
TABLE NAMES GIVGEN BELOW:

.GRANTED_PRIVILIGES -- list granted privilizes to user and roles

.GRANTED_ROLES ---- lists the granted roles

.EFFECTIVE_ROLES

.EFFECTIVE_PRIVILIGES

.M_LOG_SEGMENTS --- Information on log segmenents size,type,volume and its backup information

.M_VOLOUME_IO_STATISTICS

.M_SERVICE_MEMORY

.M_HEAP_MEMORY_RESET

.M_CS_TABLES --- Lists column store tables

.M_RS_TABLES --- List row store tables

.M_HOST_RESOURCE_UTILIZATION --- List resource utilized information by host

.M_DELTA_MERGE_STATISTICS   --- Information related to Delta Merge operation


.GLOBAL_MEMORY_STATITICS --- 

.M_EXPORT_STATUS ---- Table export information

.M_IMPORT_BINARY_STATUS --- Status of import operation of table

.M_BACKUP_CATALOG --- Overview of backup information with backup id,mode,type,status

.M_BACKUP_CATALOG_FILES --- Overview of backup catalo9g with source and destinatio0n information

.M_BACKUP_PROGRESS --- Info, related to recent complete data backup

.M_SERVICE_REPLICATION ---  Provides status of system replication adn log shipping information.

.INVALID_COMMECT_ATTEMPTS --- Provides information related to last invalid connect to DB by user

.STRUCTURED_PRIVILIGES ---  Provides view of structured privilizes (Analytical previlges)

SELECT * FROM AUDIT_ACTIONS ORDER BY action_group, action_name;.

Syntax to create audit policy
CREATE AUDIT POLICY <policy_name> AUDITING <audit_status> <audit_actions> LEVEL <audit_level> <opt_audit_trail_type>

M_CUSTOMIZABLE_FUNCTIONALITIES
