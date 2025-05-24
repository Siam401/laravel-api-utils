# File-Upload

A simple package to help you easily structure api for your laravel project.

---

## Installation

You can install the package via Composer:

```bash
composer require siam401/apiutil
```

#Code example


```php
use Siam401\ApiUtil\ApiUtil;

return FileUpload::upload('file'); // single or multiple file upload
return FileUpload::getUrl('file-path');
return FileUpload::render('file-path');
return FileUpload::remove('file-path');
return FileUpload::removeDirectory('file-path');
return FileUpload::storagePath('file-path');
return FileUpload::exists('file-path');
return FileUpload::getUploadTime('file-path');
```
