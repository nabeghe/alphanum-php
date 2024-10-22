# Alphanum for PHP.

> Converting decimal numbers to alphanums, which include uppercase & lowercase letters as well as the underscore character, & vice versa.

**Notice:** It's useful for shortening links by converting post numbers to alphanumeric characters.

<hr>

## 🫡 Usage

### 🚀 Installation

You can install the package via composer:

```bash
composer require nabeghe/colory
```

<hr>

#### Example:

```php
<?php

require 'vendor/autoload.php';

use Nabeghe\Alphanum\Alphanum;

echo "[[ To Alphanum ]]\n";
echo '0 => '.Alphanum::generate(0)."\n"; // 0
echo '1 => '.Alphanum::generate(1)."\n"; // 1
echo '10 => '.Alphanum::generate(10)."\n"; // A
echo '11 => '.Alphanum::generate(11)."\n"; // B
echo '12 => '.Alphanum::generate(12)."\n"; // C
echo '13 => '.Alphanum::generate(13)."\n"; // D
echo '14 => '.Alphanum::generate(14)."\n"; // E
echo '100 => '.Alphanum::generate(100)."\n"; // 1f
echo '1000 => '.Alphanum::generate(1000)."\n"; // Gf
echo '1403 => '.Alphanum::generate(1403)."\n"; // NN
echo '2024 => '.Alphanum::generate(2024)."\n"; // Yj
echo '1000000 => '.Alphanum::generate(1000000)."\n"; // 4clf
echo '1000000000 => '.Alphanum::generate(1000000000)."\n"; // 1H9clf
echo 'PHP_INT_MAX => '.Alphanum::generate(PHP_INT_MAX)."\n"; // FFDZXWuKFV7
echo "\n";

echo "[[ To Decimal ]]\n";
echo '0 => '.Alphanum::toDecimal('0')."\n"; // 0
echo '1 => '.Alphanum::toDecimal('1')."\n"; // 1
echo 'A => '.Alphanum::toDecimal('A')."\n"; // 10
echo 'B => '.Alphanum::toDecimal('B')."\n"; // 11
echo 'C => '.Alphanum::toDecimal('C')."\n"; // 12
echo 'D => '.Alphanum::toDecimal('D')."\n"; // 13
echo 'E => '.Alphanum::toDecimal('E')."\n"; // 14
echo '1f => '.Alphanum::toDecimal('1f')."\n"; // 100
echo 'Gf => '.Alphanum::toDecimal('Gf')."\n"; // 1000
echo 'NN => '.Alphanum::toDecimal('NN')."\n"; // 1403
echo 'Yj => '.Alphanum::toDecimal('Yj')."\n"; // 2024
echo '4clf => '.Alphanum::toDecimal('4clf')."\n"; // 1000000
echo '1H9clf => '.Alphanum::toDecimal('1H9clf')."\n"; // 1000000000
echo 'FFDZXWuKFV7 => '.Alphanum::toDecimal('FFDZXWuKFV7')."\n"; // PHP_INT_MAX
echo "\n";
```

<hr>

## 📖 License

Copyright (c) 2024 Hadi Akbarzadeh

Licensed under the MIT license, see [LICENSE.md](LICENSE.md) for details.