# Crear directorios
mkdir /dir/to/stable_24/moodle
mkdir /dir/to/stable_24/moodledata

# Establecer enlace simbólico
ln -s /dir/to/stable_24/moodle /var/www/stable_24

# Clonar el repositorio de Moodle
git clone git://git.moodle.org/moodle.git /dir/to/moodle

# Navegar al directorio de Moodle
cd /dir/to/stable_24/moodle

# Instalar Moodle con parámetros personalizados
php admin/cli/install.php --wwwroot "http://localhost/stable_24" --dataroot /dir/to/stable_24/moodledata --dbtype pgsql --dbname stable24 --dbuser root --dbpass root --dbhost localhost --fullname "Stable 24 PostgreSQL" --shortname stable_24 --adminuser admin --adminpass test --allow-unstable --agree-license --non-interactive

# Editar el archivo de configuración de Moodle
vim config.php

# Agregar las siguientes configuraciones:
$CFG->sessioncookiepath = '/stable_24/';
$CFG->debug = DEBUG_DEVELOPER;
$CFG->debugdisplay = 1;
$CFG->passwordpolicy = 0;
$CFG->perfdebug = 15;
$CFG->debugpageinfo = 1;
$CFG->allowthemechangeonurl = 1;
$CFG->cachejs = 0;
$CFG->yuicomboloading = 0;
