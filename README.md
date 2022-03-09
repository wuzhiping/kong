https://github.com/pantsel/konga

psql -U kong -d kong

create database konga

docker-compose run konga -c prepare -a postgres -u postgresql://kong:kong@kong-database:5432/konga
