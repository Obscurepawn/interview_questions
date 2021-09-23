<!--
 * @Author: uestc.zyj@gmail.com
 * @Date: 2021-09-23 11:02:53
 * @LastEditTime: 2021-09-23 19:14:04
 * @Description: linux shell questions
 * @FilePath: /interviews/shell/shell.md
-->

常考的一般是让你统计出现次数最多的ip地址,对xx进行统计并输出前x名之类的。

常用的命令有以下几个

- cat [文件名] (输出某个文件的内容)
- awk '{[条件] [行动]}' (例如 awk '{if ($1>100) print $0}' 是指如果第一列的数字大于100则输出一整行。)
- cut -d [分割符] -f [列数]  例如(cut -d ':' -f 1 则是以:为分隔符，分割后取第一行)
- sort (按照字典序排序)
- uniq -c (去重且计算每个元素出现的次数)
- sort -rn (根据uniq -c的结果进行排序)
- head -n [行数] (只显示前x行)
- wc (统计行数，字数，字节数)
