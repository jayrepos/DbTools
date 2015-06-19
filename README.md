# DbTools

Class to be able to use MySQL specific functions into a Symfony 2 Doctrine project:
- DAYOFWEEK() - https://dev.mysql.com/doc/refman/5.5/en/date-and-time-functions.html#function_dayofweek
- TIME_TO_SEC() - https://dev.mysql.com/doc/refman/5.5/en/date-and-time-functions.html#function_time-to-sec

Add theses lines to you config.yml file
```
doctrine:
  orm:
    entity_managers:
      default:
        dql:
          datetime_functions:
            day_of_week:  DbTools\DayOfWeek
```
