# discourse-settings-uploader
Install a Discourse settings JSON file to a site


### To create/retrieve settings

Create a JSON settings dump by visiting https://discourse.example.com/admin/site_settings.json and saving the file somewhere convenient.

Retrieve your site's API key from https://discourse.example.com/admin/api/keys

### To install these settings to another site

Do this:

   ./discourse-settings-uploader HOSTNAME API_KEY API_USER SETTINGS_FILE

For example:

   ./discourse-settings-uploader discourse.example.com d35989078a system site_settings.json

### Warning

This script does no error checking and could destroy your site, cause fires, or hurt people.

You should make a backup of your site before you use this script.

You can, at your own peril, edit the JSON file before running the script, but note that no error checking is done, so you should make a backup of the original settings file too.
