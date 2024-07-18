# Top-Spotify-Songs-2024
--Indentifying Data integrity
SELECT * FROM spotify_songs.`top _spotify_songs`;

--count the no of rows
SELECT COUNT(*) FROM spotify_songs.`top _spotify_songs`;

-- This command will display the structure of the table, including the names of columns, their data types, whether they allow null values, and any additional attributes like auto-increment or primary key.
DESCRIBE spotify_songs.`top _spotify_songs`;
DESC spotify_songs.`top _spotify_songs`;

-- Identify missing values
SELECT * FROM spotify_songs.`top _spotify_songs` 
WHERE `Track` IS NULL 
OR `Album Name` IS NULL 
OR `Artist` IS NULL 
OR `Release Date` IS NULL 
OR `Spotify Streams` IS NULL 
OR `YouTube Likes` IS NULL;
