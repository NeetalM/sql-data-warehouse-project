/*
=====================================================================
CREATE TABLES & RENAME TABLES
=====================================================================
*/

CREATE TABLE bronze.crm_cust_info (
cst_id INT,
cst_key NVARCHAR(50),
cst_firstname NVARCHAR(50),
cst_lastname NVARCHAR(50),
cst_material_status NVARCHAR(50),
cst_gndr NVARCHAR(50),
cst_create_date DATE);

CREATE TABLE bronze.crm_prd_info (
prd_id INT,
prd_key VARCHAR(50),
prd_nm VARCHAR(50),
prd_cost INT,
prd_line VARCHAR(50),
prd_start_dt DATE,
prd_end_dt DATE);

CREATE TABLE bronze.sales_details (
sls_ord_num VARCHAR(50),
sls_prd_key VARCHAR(50),
sls_cust_id INT,
sls_order_dt DATE,
sls_ship_dt DATE,
sls_due_dt DATE,
sls_sales INT,
sls_quantity INT,
sls_price INT);

DROP TABLE bronze.sales_details;

CREATE TABLE bronze.sales_details (
sls_ord_num VARCHAR(50),
sls_prd_key VARCHAR(50),
sls_cust_id INT,
sls_order_dt INT,
sls_ship_dt INT,
sls_due_dt INT,
sls_sales INT,
sls_quantity INT,
sls_price INT);

CREATE TABLE bronze.CUST_AZ12 (
CID VARCHAR(50),
BDATE DATE,
GEN VARCHAR(50)
);

EXEC sp_rename 'CUST_AZ12', 'erp.CUST_AZ12';

CREATE TABLE bronze.LOC_A101 (
CID VARCHAR(50),
CNTRY VARCHAR(50));

EXEC sp_rename 'bronze.CUST_AZ12', 'erp_cust_az12';
EXEC sp_rename 'bronze.LOC_A101', 'erp_loc_a101';

CREATE TABLE bronze.erp_px_cat_g1v2 (
ID VARCHAR(50),
CAT VARCHAR(50),
SUBCAT VARCHAR(50),
MAINTENANCE VARCHAR(50));
