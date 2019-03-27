


    docker-compose run web rails new . --force --no-deps --database=postgresql

    sudo chown -R $USER:$USER .

    docker-compose build

Replace the contents of config/database.yml with the following:

         default: &default
           adapter: postgresql
           encoding: unicode
           host: db
           username: postgres
           password:
           pool: 5
         
         development:
           <<: *default
           database: myapp_development
         
         
         test:
           <<: *default
           database: myapp_test
         

after
docker-compose up

Finally, you need to create the database. In another terminal, run:

        docker-compose run web rake db:create