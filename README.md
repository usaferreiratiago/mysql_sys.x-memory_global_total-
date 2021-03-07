# mysql_sys.x-memory_global_total-

SELECT 
    SUM(`performance_schema`.`memory_summary_global_by_event_name`.`CURRENT_NUMBER_OF_BYTES_USED`) AS `total_allocated`
FROM
    `performance_schema`.`memory_summary_global_by_event_name`
