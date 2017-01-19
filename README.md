# wordpress-tips

## Run through a dev database to update fields with production-ready values

### Backup Database first!  

UPDATE `wp_options` SET `option_value` = replace(`option_value`,'FIND','REPLACEWITH');  
UPDATE `wp_postmeta` SET `meta_value` = replace(`meta_value`,'FIND','REPLACEWITH');  
UPDATE `wp_posts` SET `post_content` = replace(`post_content`,'FIND','REPLACEWITH');  
UPDATE `wp_posts` SET `post_title` = replace(`post_title`,'FIND','REPLACEWITH');  
UPDATE `wp_posts` SET `post_name` = replace(`post_name`,'FIND','REPLACEWITH');  
UPDATE `wp_posts` SET `guid` = replace(`guid`,'FIND','REPLACEWITH');  
