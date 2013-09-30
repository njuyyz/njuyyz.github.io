---
layout: post
title: "[ctci]Arrays and Strings"
date: 2013-09-30 10:53
comments: true
categories: 学习 CTCI
---
昨天又从[CTCI]第一章开始看了。复习了一下collections在java中实现和应用。
<!-- more -->
>
####**equals( ) and ==**

>######1. A.equals(B) compares the values of A and B, if the values of A and B are the same, return true, else return false.

>######2. A == B compares the references of A and B, if the references of A and B are the same one, return true, else return false.

>######3. if you want to override the method of equals(), you should also override the method of hashcode(), in order to maintain the contract that if two objects equal, their hashcode() should be the same.
	

***
**Hashmap Hashtable Hashset**
	
>######1. Hashtable is synchronized while Hashmap is not. So if it is thread safe, we should use Hashmap to lift the performance of our code.
	
>######2. Besides differences on Synchronized, Hashmap allows to have one null key and null values, but Hashtable does not allow to have null key or null value.
	
>######3. Hashset is a kind of set which does not allow duplicate value in a single set.
	
***
**ArrayList Vection LinkedList**
	
>######1. ArrayList and Vection are based on array, which have fixed length, if once we need to expand the size of ArayList of Vection, we need to allocate a new array, and copy the previous values into the new one.
	
>######2. ArrayList is not Synchronized, while Vector is.
	
>######3. LinkedList is based on linkedlist.
	
***
**String**

>######1. String objects can not be modified once it was created.
	
>######2. String is a final class, cannot have subclass.
	
>######3. If a String object is ofen modified through its life cycle, we should use StringBuffer( or StringBuilder).
	
>######4. StringBuilder is faster, because it is not Synchronized, while StringBuffer is.
	 
	 