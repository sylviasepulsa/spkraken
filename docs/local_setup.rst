K****n Installation Guide
=========================

Local Installation
-------------------
1. Clone repo https://github.com/s*****a/k****n.git outside of docroot
2. Use drush to create local folder in docroot

   .. code:: 
   
      $ drush make k****n.make <destination_folder>

3. Link github cloned folder to docroot folder

   .. code:: 

     $  ln -s <github_repo_folder>/modules <k****n_docroot_folder>/sites/all/modules/custom
     $  ln -s <github_repo_folder>/profiles/k****n_dev <kraken_docroot_folder>/profiles

4. Write github_repo_folder and kraken_docroot_folder complete
5. Import k****n database

   .. code:: 

     $  drush -v --root=/Applications/XAMPP/htdocs/k****n si k****n_dev --db-url=mysql://drupal:drupal@localhost/k****n --account-name=admin --account-pass=admin -y
     $  drush en date_views views_bulk_operations views_data_export views_date_format_sql views_megarow views_ui queue_ui -y
     $  drush sql-cli < /k****n/scripts/assets/k****n_dev.sql


Local Installation with Docker 
------------------------------

1. Download docker from official page here_ , then install Docker.dmg

   .. _here: https://docs.docker.com/docker-for-mac/install/#download-docker-for-mac

2. Make sure the docker engine is running
3. Clone repo kraken_

   .. _kraken: https://github.com/s*****a/k****n
   
4. Open terminal/bash script, then go to download folder  ``$ cd /folder1/folder2/k****n``
5. Built image  ``$ docker-compose up``

  .. note:: 
     - Show version : ``- $docker version``
	   - Show info : ``- $ docker ps -a`` 
	   - Running docker daemon mode : ``- $ docker-compose up -d``
	   - Stop docker : ``- $ docker-compose stop``
	   - get ``bash/shell`` into running container ``- $ docker exec -i -t 'NAMES' /bin/bash``



K****n Features
================

K****n is bla bla bla. K****n can be accessed through this link ``https://k****n.s****a.id/``. K***** has several Menus, such as:

* Menu A
* Menu B
* Menu C

