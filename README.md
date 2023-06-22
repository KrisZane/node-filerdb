# Filer DB

Basic nosql database, based on JSON and filesystem features. This is meant for journaling and replecative filesystems like ext4 and zfs.

## The Idea

Part of the reason databases were created in the first place, was due to slow read/write media and to maintain and monitor data integrity.

With SSD's being more commonplace and filesystem such as ZFS implenting natural data integrity and ease of backups, the need for data integrity checks is not as important as it used to be.

On top of this the rise of microservices and online object storage (like S3), has mostly removed the need to always have a database system.

The idea then became, why not have a simplified file/object storage based database, with simple but efficient indexing. Giving people flexibility of where to put their storage, but also the simplicity of using files/objects.

The setup allows to distribute files/objects into object stores, inside of microservices and even to be hosted in CDN's or direct downloads from Apache/Nginx/OLS.