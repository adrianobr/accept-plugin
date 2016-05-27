# Redmine Accept Plugin
People having worked with TRAC are used to "accept" issues, which basically states that someone will now actively work on a specific issue. Redmine apparently also supports custom issue statuses, such as "accepted", but it requires more than one click to accept an issue (edit issue, select status "accepted", select assignee). This plugin allows to accept tickets with one click.

### Installation Notes
The plugin can be installed as ordinary redmine plugin (compatible with redmine 3.2.x, 3.0.x, 2.6.x) and does not require database migration:
* Create directory your_redmine_base/plugins/accept
* Copy the content of this repository to the created directory
* Restart redmine (e.g., through "touch your_redmine_base/tmp/restart.txt)
* The accept plugin needs to know which issue status is considered as "accepted" in your redmine installation. By default, the first status is considered the "accepted" status. This behaviour can be configured in your redmine installation: Administration --> Plugins --> Accept Plugin --> Configure

### Version History

0.0.2
* Allows the accept status to be dependent on the tracker the issue is assigned to, see [#5](../../issues/5). 

0.0.1 
 * First version of the plugin.
