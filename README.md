# becloudready

**required modules <br>
django : framework <br>
psycopg : PostgreSQL database adapter for the Python <br>
subprocess : executing remote python scripts

**process
-----------------------------------------------------------------------
1.setting up django project
2.adding postgresql as database
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'guest_book',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
3.creating model with requires attributes
4.Create Serializer class for Data Model
5.creating API functions for CRUD operations
----------------------------------------------------------------------
**weather.py
1.creating new python script that executes remote python scripts using subprocess module
from subprocess import call
call(["python","file_name.py"])
                               Day                          Description            Temperature
0                          Tonight      A clear sky and a gentle breeze             Low23° 74°
1      Friday 22nd OctoberFri 22nd  Sunny intervals and a gentle breeze  High33° 92°Low23° 74°
2    Saturday 23rd OctoberSat 23rd  Sunny intervals and a gentle breeze  High32° 90°Low23° 74°
3      Sunday 24th OctoberSun 24th  Sunny intervals and a gentle breeze  High32° 90°Low23° 74°
4      Monday 25th OctoberMon 25th  Sunny intervals and a gentle breeze  High32° 89°Low24° 75°
5     Tuesday 26th OctoberTue 26th  Sunny intervals and a gentle breeze  High33° 90°Low24° 76°
6   Wednesday 27th OctoberWed 27th  Sunny intervals and a gentle breeze  High34° 93°Low24° 76°
7    Thursday 28th OctoberThu 28th  Sunny intervals and a gentle breeze  High34° 93°Low24° 76°
8      Friday 29th OctoberFri 29th  Sunny intervals and a gentle breeze  High34° 93°Low25° 76°
9    Saturday 30th OctoberSat 30th  Sunny intervals and a gentle breeze  High34° 93°Low25° 76°
10     Sunday 31st OctoberSun 31st  Sunny intervals and a gentle breeze  High34° 93°Low24° 76°
11      Monday 1st NovemberMon 1st      Light cloud and a gentle breeze  High34° 93°Low25° 76°
12     Tuesday 2nd NovemberTue 2nd      Light cloud and a gentle breeze  High33° 92°Low25° 76°
13   Wednesday 3rd NovemberWed 3rd      Light cloud and a gentle breeze  High33° 92°Low24° 76°

the above response is send to html page and displayed in tabular format as i did in my <a href="http://visualdashboard.herokuapp.com/">previous project</a>
