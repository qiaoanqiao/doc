---
title: Time
meta:
  - name: description
    content: 时间戳助手
  - name: keywords
    content: easyswoole|组件库|杂项工具|Time
---



# Time



## 用途

时间戳助手



## 核心对象类

实现该组件功能需加载核心类：

```php
EasySwoole\Utility\Time
```



## 核心对象方法



#### startTimestamp

返回某一天开始的时间戳

- mixed $date 字符串日期或时间戳

```php
static function startTimestamp($date = '')
```

:::tip

例子

:::

```php
<?php
/**
 * Created by PhpStorm.
 * User: root
 * Date: 19-1-9
 * Time: 上午10:10
 */

require './vendor/autoload.php';

var_dump(\EasySwoole\Utility\Time::startTimestamp('2019-4-15'));

/**
 * 输出结果:
 * int(1555286400)
 */
```



#### endTimestamp

返回某一天结束的时间戳

- mixed $date 字符串日期或时间戳

```php
static function endTimestamp($date = '')
```

:::tip

例子

:::

```php
<?php
/**
 * Created by PhpStorm.
 * User: root
 * Date: 19-1-9
 * Time: 上午10:10
 */

require './vendor/autoload.php';

var_dump(\EasySwoole\Utility\Time::endTimestamp('2019-4-15'));

/**
 * 输出结果:
 * int(1555372799)
 */
```



#### endTimestamp

从字符串创建出 Datetime 对象

- mixed $datetime 传入文本日期或者时间戳

```php
static function createDateTimeClass($datetime = '')
```

:::tip

例子

:::

```php
<?php
/**
 * Created by PhpStorm.
 * User: root
 * Date: 19-1-9
 * Time: 上午10:10
 */

require './vendor/autoload.php';

var_dump(\EasySwoole\Utility\Time::createDateTimeClass('2019-4-15'));

/**
 * 输出结果:
 * object(DateTime)#3 (3) {
 *   ["date"]=>
 *   string(26) "2019-04-15 00:00:00.000000"
 *   ["timezone_type"]=>
 *   int(1)
 *   ["timezone"]=>
 *   string(6) "+00:00"
 * }
 */
```



#### parserDateTime

从DateTime对象中获取年月日时分秒

- mixed $datetime 传入文本日期或者时间戳

```php
static function parserDateTime($dateTime)
```

:::tip

例子

:::

```php
<?php
/**
 * Created by PhpStorm.
 * User: root
 * Date: 19-1-9
 * Time: 上午10:10
 */

require './vendor/autoload.php';

var_dump(\EasySwoole\Utility\Time::parserDateTime('2019-4-15'));

/**
 * 输出结果:
 * array(6) {
 *   [0]=>
 *   string(2) "00"
 *   [1]=>
 *   string(2) "00"
 *   [2]=>
 *   string(2) "00"
 *   [3]=>
 *   string(1) "4"
 *   [4]=>
 *   string(2) "15"
 *   [5]=>
 *   string(4) "2019"
 * }
 */
```

