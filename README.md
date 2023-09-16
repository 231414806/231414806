mkdir /dir/to/stable_24/moodle
mkdir /dir/to/stable_24/moodledata
ln -s /dir/to/stable_24/moodle /var/www/stable_24
git clone git://git.moodle.org/moodle.git /dir/to/moodle
cd /dir/to/stable_24/moodle
php admin/cli/install.php --wwwroot## "http://localhost/stable_24" --dataroot/dir/to/stable_24/moodledata --dbtype## pgsql --dbnamestable24 --dbuser## root --dbpassroot --dbhost## localhost --fullname"Stable 24 PostgreSQL" --shortname## stable_24 --adminuseradmin --adminpass=test --allow-unstable --agree-license --non-interactive
vim config.php
# Add the following settings:
# - $CFG->sessioncookiepath: /stable_24/
# - $CFG->debug: DEBUG_DEVELOPER
# - $CFG->debugdisplay: 1
# - $CFG->passwordpolicy: 0
# - $CFG->perfdebug: 15
# - $CFG->debugpageinfo: 1
# - $CFG->allowthemechangeonurl: 1
# - $CFG->cachejs: 0
# - $CFG->yuicomboloading: 0
# Include FirePHP Core
# Login to Moodle
# Create 10 students, 3 teachers and 3 managers
