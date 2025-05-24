# API Utils for Laravel

A simple Laravel helper to standardize API JSON responses.

## 📦 Installation

```bash
composer require siam401/api-utils
```

## 🚀 Usage

Import the class:

```php
use Siam401\ApiUtils\ApiUtil;
```

### ✅ Success Response

```php
return ApiUtil::success('Fetched successfully', $data);
```

### ❌ Failure Response

```php
return ApiUtil::failure('Something went wrong', 400, ['field' => 'error']);
```

### 💥 Crash Response

```php
return ApiUtil::crash('Unexpected system error', 500, ['exception' => $e->getMessage()]);
```

### 🔍 Not Found Response

```php
return ApiUtil::notFound('Record not found');
```

## 📁 Response Format

All responses follow a consistent structure:

```json
{
  "message": "Description",
  "contents": {...}
}
```

## 🛠️ Requirements

- PHP ^8.0
- Laravel 9 or 10

## 📄 License

This package is open-source software licensed under the [MIT license](LICENSE).
