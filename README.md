# This skeleton is only for deploy in digitalocean

Follow the next instructions after clone the repo:

1. In settings file change database password to the database password that digitalocean give you.
2. run the next command, remember change the droplet ip_address in the command
    ```
    $ git remote add production ssh://root@<droplet ip_address>/home/django/repo
    ```
3. Run the next command to deploy to production:
    ```
    $ git push production master
    ```

If you want use develop settings follow the next instruction, remember that settings file has production credentials and local_settings has your local credentials

1. Inside of django_project folder rename the file `local_settings.py.example` to `local_settings.py`
