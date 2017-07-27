# MyPacd_7.24_oracle


update pacd.PACD_SPOKETRAINER_T
set doc_id = concat(doc_id, ',');
where not REGEXP_LIKE(doc_id, '/,$');


where doc_id not like '%,'
