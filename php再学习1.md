---
title: php再学习1
date: 2016-05-24 14:28:34
tags: [php,strpos,strtoupper]
---
## 字符串函数
## strpos (查找字符串首次出现的位置 )
>   mixed  strpos  ( string $haystack  , mixed  $needle  [, int $offset  = 0  ] )
返回 needle 在 haystack 中首次出现的数字位置。 

### 参数介绍
 - haystack （在该字符串中进行查找。）
 - needle （如果needle不是一个字符串，那么他将被转换成整形并视为字符的顺序值）
 - 如果提供了此参数，搜索会从字符串该字符数的起始位置开始统计
###返回值
返回 needle 存在于 haystack 字符串起始的位置(独立于 offset)。同时注意字符串位置是从0开始，而不是从1开始的。 如果没找到 needle，将返回 FALSE 。 
+ <!-- more -->
<The rest of contents | 余下全文>

### example 
    <?php
    $mystring  =  'abc' ;
    $findme    =  'a' ;
    $pos  =  strpos ( $mystring ,  $findme );
     // 注意这里使用的是 ===。简单的 == 不能像我们期待的那样工作，
    // 因为 'a' 是第 0 位置上的（第一个）字符。
    if ( $pos  ===  false ) {
        echo  "The string ' $findme ' was not found in the string ' $mystring '" ;
    } else {
        echo  "The string ' $findme ' was found in the string ' $mystring '" ;
        echo  " and exists at position  $pos " ;
    }
    ?> 

## strtoupper （将字符串转化成大写）
>string strtoupper  ( string $string  )
将 string 中所有的字母字符转换为大写并返回。 

## strtolower  （将字符串转化为小写 ）
>string strtolower  ( string $string  )
将 string 中所有的字母字符转换为小写并返回。

## explode (使用一个字符串分割另一个字符串)
>array explode  ( string $delimiter  , string $string  [, int $limit  ] )
此函数返回由字符串组成的数组，每个元素都是 string 的一个子串，它们被字符串 delimiter 作为边界点分割出来。 

### 参数
 - delimiter (分割字符)
 - string (被分割字符串)
 - limit (分割后的结果个数)
###返回值 
返回由字符串组成的数组



