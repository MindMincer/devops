| Variable        | value           |
| ------------- |-------------:|
|app_name| my_uwsgi_app|
|app_package| wsgi|
|app_callable| app|
|base_dir| '/srv/{{ app_name }}'|
|appdata_dir| '{{ base_dir }}/appdata'|
|nginx_server_name| 'localhost'|
|nginx_http_port| 80|
|uwsgi_module| '{{ app_package }}:{{ app_callable }}'|
|uwsgi_processes| 1|
|uwsgi_threads| 1|
|uwsgi_env| []|
|git_repo| https://github.com/MindMincer/devops|
|git_branch| master|
|uid| uwsgi|
|gid| nginx|
|nginx_dir| /etc/nginx/conf.d|
|uwsgi_dir| /etc/uwsgi.d|
|uwsgi_plugins| python3,logfile|
|virtualenv_cmd| python3 -m virtualenv|
|uwsgi_service_name| uwsgi|
