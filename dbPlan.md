universe

galaxy
- galaxy_id
  - PRIMARY KEY
- name
  - varchar 30
  - UNIQUE
  - NOT NULL
- diameter (kly)
  - INT
- apparent magnitude
  - NUMERIC(4,2)
- distance (kly)
  - INT

star
- star_id
- name
  - varchar
  - UNIQUE
  - NOT NULL
- galaxy_id
- distance (ly)
  - INT
- stellar_class
  - TEXT


planet
- planet_id
- name
  - varchar
  - UNIQUE
  - NOT NULL
- mass
  - NUMERIC(6,2)
- inclination_known
  - BOOLEAN
- star_id


moon
- mood_id
- name
  - varchar
  - UNIQUE
  - NOT NULL
- mean_radius(km)
  - INT
- year_discovered
  - TEXT
- planet_id


asteroid
- asteroid_id
- name
  - varchar
  - UNIQUE
  - NOT NULL
- dimensions_known
  - BOOLEAN
- star_id
