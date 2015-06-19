# DbTools

This is a class to be able to use DAYOFWEEK() function of MySQL into a Symfony 2 project

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
