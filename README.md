# ptreodactyl-thema-glow
'''cd /var/www/pterodactyl'''
curl -L -o panel.tar.gz "https://github.com/wanzofc-dev/ptreodactyl-thema-glow/raw/main/panel.tar.gz"
tar -xzvf panel.tar.gz
rm panel.tar.gz
php artisan view:clear
php artisan cache:clear
chown -R www-data:www-data /var/www/pterodactyl/*
