---
title: My Note's Title
tags: misc, sublime
notebook: My Notebook 
date: 2017/1/6 15:38:00
---
# LuCardView
##简介咯
这是一个可扩展的CardView。先上一个效果图。
![Alt text](image/CardView1.png)
这个CardView分为上下两部分，上部分为Title部分，包括一个Title和一个Summary字符串和一个箭头。

下部分则是Content部分。

通过点击Title部分可以展开和关闭CardView并与上下产生一个margin值。

##使用方法
下载lucardview文件夹，Android studio中导入Module就行了...

```xml
    <com.beginlu.lucardview.LuCardView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:summary="summary"
        app:title="title">

        <RelativeLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:padding="@dimen/activity_horizontal_margin">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="content" />
        </RelativeLayout>
    </com.beginlu.lucardview.LuCardView>
```
##PS
展示发现了一些Bug，待解决。

- Content内容为空时CardView无法展示。
- 箭头是文字的>太丑了