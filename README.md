# vivo-sync
Syncing files between the vivo prod server and test server

Sync from the vivo server to your desired destination. The `-t` flag tracks the time the file was created. The `-x` flag prevents rsync from copying mounted directories. The `-r` flag makes the sync recurse into directories.

`rsync -txr user@vivo.ufl.edu:/usr/local/vdata/uploads/file_storage_root /my/path/to/synced/folder`

To delete files that are in the destination but not in the origin, add the `--delete` flag.
