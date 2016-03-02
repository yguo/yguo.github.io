---
layout: inner
title: Lessons
permalink: /lessons/
---

### 10 Java Common Mistakes beginners made

--

Beginners don't follow the rules: Creating objects only when it is necessary. Here is an example:

```java
public class Person {
    public boolean hasFollowedLeifeng(){
        Calendar gmtCal = Calendar.getInstance(TimeZone.getTimeZone("GMT"));
        gmtCal.set(1950, Calendar.JANUARY, 1, 0, 0, 0);
        Date leifengStart = gmtCal.getTime();
        gmtCal.set(1983, Calendar.JANUARY, 1, 0, 0, 0);
        Date lefengEnd = gmtCal.getTime();
        return birthDate.compareTo(leifengStart) >= 0 && 
               birtheDate.compareTo(leifengEnd) < 0 ;
    }
}
```

{% highlight java %}
public class Person {
    public boolean hasFollowedLeifeng(){
        Calendar gmtCal = Calendar.getInstance(TimeZone.getTimeZone("GMT"));
        gmtCal.set(1950, Calendar.JANUARY, 1, 0, 0, 0);
        Date leifengStart = gmtCal.getTime();
        gmtCal.set(1983, Calendar.JANUARY, 1, 0, 0, 0);
        Date lefengEnd = gmtCal.getTime();
        return birthDate.compareTo(leifengStart) >= 0 && 
               birtheDate.compareTo(leifengEnd) < 0 ;
    }
}
{% endhighlight %}