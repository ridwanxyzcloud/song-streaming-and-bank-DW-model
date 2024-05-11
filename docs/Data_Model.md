# AudioCloud Data Warehouse - Data Model

This document describes the data model used in the AudioCloud data warehouse. The data model is designed to efficiently store and manage data related to user activities, song metadata, playlists, and more.

## Entity-Relationship Diagram

Insert ER Diagram image here

## Tables

### users
- user_id (Primary Key, Integer)
- username (Text)
- email (Text)
- registration_date (Date)
- ...

### songs
- song_id (Primary Key, Integer)
- title (Text)
- artist_id (Integer, Foreign Key)
- genre (Text)
- duration (Integer)
- ...

### playlists
- playlist_id (Primary Key, Integer)
- user_id (Integer, Foreign Key)
- name (Text)
- creation_date (Date)
- ...

... (continue describing other tables)
