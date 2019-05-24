---
layout: post
title:  "Making a diamond with Star"
date:   2019-05-23 08:45:00
author: Pray Lee
categories: Java
tags: programming diamond star
---


It's my First post about java programming.
Also i hope that i will keep the posting.

### Code 

{% highlight java %}
import java.util.Scanner;

public class MakingStarRibbon {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String star = "*";
		String under = "_";
		String test = "&";
		int i;
		int j=0;
		int k;
		int l;
		int n;
		int count=0;
		System.out.print("Insert Number >> ");
		int max = sc.nextInt(); 
		for(i=0 ; i<(max); i++) {
			if(i<(max+1)/2){
				j++;
			}if(i>(max)/2) {
				j--;
			}
			for(k=0; k<j;k++) {
				System.out.print(star);
				count++;
			}
			for(l=0;l<max-j*2;l++) {
				System.out.print(under);
				count++;
			}
			for(n=0; n<max-count;n++) {
				System.out.print(star);
			}
			System.out.println();
			count = 0;
		}
	}
}
{% endhighlight %}
