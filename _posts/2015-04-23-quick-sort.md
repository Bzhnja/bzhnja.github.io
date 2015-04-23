---
layout:post
title: Quick sort
categories:
  - Algorithm
tags:
  - sort
  - quick_sort
  - c++_code
comments: true
---

       void quick_sort(int *a, int left, int right){
    		if(left>right) return;
    		int pivot = a[left];
    		int temp, i=left, j=right;
    		while(i!=j){
    			while(a[j]>=pivot&&j>i) j--;
    			while(a[i]<=pivot&&i<j) i++;
    			if(i<j){
    				temp = a[i];
    				a[i] = a[j];
    			a[j] = temp;
    			}
    		}
    		a[left] = a[i];
    		a[i] = pivot;
    		quick_sort(a,left,i-1);
    		quick_sort(a,i+1,right);
    	}