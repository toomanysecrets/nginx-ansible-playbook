
Manuel Trujillo 06/Junio/2025
Preparación para una instalación de servidores con Nginx
con atención a systemd, control con systemd watchdog y timer (además de
reinicio propio ante fallos por systemd).
También incorpora política SELinux para contenido HTTP/HTTPS

nginx-playbook/
├── inventory
├── playbook_nginx.yml
└── roles/
    └── nginx/
        ├── tasks/
        │   └── main.yml
        ├── files/
        │   ├── nginx-override.conf
        │   ├── nginx-watchdog.timer
        │   └── nginx-watchdog.service

