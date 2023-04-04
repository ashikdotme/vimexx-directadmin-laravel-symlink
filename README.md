# vimexx-directadmin-laravel-symlink
#web.php
```
Route::get('/link-storage', function () {
    $targetFolder = base_path().'/storage/app/public';
    $linkFolder = $_SERVER['DOCUMENT_ROOT'].'/storage';
    symlink($targetFolder, $linkFolder); 
});

```

# Cpanel Hosting Symlink for Laravel Application
#### Create a symlink.php file then write bottom code after that run the symlink.php file.
```
<?php 
symlink('/home/backoffice/storage/app/public', '/home/public_html/storage'); 
echo 'Symlink process successfully completed';
?>
```
