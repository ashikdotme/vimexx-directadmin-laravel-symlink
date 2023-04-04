# vimexx-directadmin-laravel-symlink


#web.php
```
Route::get('/link-storage', function () {
    $targetFolder = base_path().'/storage/app/public';
    $linkFolder = $_SERVER['DOCUMENT_ROOT'].'/storage';
    symlink($targetFolder, $linkFolder); 
});

```
