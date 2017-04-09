---
layout: single
title: Nháy đơn và nháy kép trong PHP
excerpt_separator: <!--more-->
thumbnail: https://namjayer.net/wp-content/uploads/2017/04/phptut.png
---
<img src="{{ post.thumbnail }}" align="center" />
<h2>Nháy đơn và nháy kép ?</h2>

Thỉnh thoảng, trong khi code PHP chắc hẳn chúng ta đã từng nhìn thấy dấu nháy đơn và nháy kép xuất hiện trong các đọan code. <!--more-->
Và ngay cả bản thân chúng ta cũng đã từng sử dụng qua lại giữa dấu nháy đơn hoặc nháy kép như một thói quen mà không hề hiểu rõ được khi nào nên dùng nháy đơn hoặc nháy kép. Bài viết này có thể sẽ giúp bạn phân biệt được khi nào nên dùng nháy đơn hoặc nháy kép

 

<h2>Dấu nháy đơn</h2>

Dấu ngoặc đơn không thể Parse được giá trị của biến.

Có nghĩa là, những gì được viết trong dấu nháy đơn sẽ được hiển thị ra y hệt mà không được Parse. Các kí hiệu như \n hoặc \t sẽ không được xác định

Ví dụ:

{% highlight php linenos %}
  // khai báo biến + giá trị
  $bien = "gia tri";
  echo 'In du lieu $bien';
{% endhighlight %}

Kết quả:

{% highlight php linenos %}
  In du lieu $bien
{% endhighlight %}

Giá trị của biến $bien không được hiểu, cho nên nó in ra chuỗi $bien chứ không in ra giá trị của biến $bien

<h2>Dấu nháy kép</h2>

Dấu nháy kép ngược lại với dấu nháy đơn. Khi bạn echo biến thì nó sẽ tìm và parse giá trị của biến.

{% highlight php linenos %}
  // khai báo biến + giá trị
  $bien = "gia tri";
  echo 'In du lieu $bien';
{% endhighlight %}

Kết quả:

{% highlight php linenos %}
  In du lieu gia tri
{% endhighlight %}


Giá trị của biến $bien được hiểu và hiển thị.

 
Tóm lại, nếu bạn muốn biến của bạn được hiểu và parse giá trị ra bên ngoài thì dùng dấu nháy kép còn nếu muốn in một chuỗi thông thường thì dùng dấu nháy đơn.

Hy vọng bài viết sẽ giúp ích được cho các bạn. Nếu ai có câu hỏi gì hay có thắc mắc gì về PHP hay SEO có thể Contact cho mình hoặc để lại Comment và đừng quên Subscribe để có thể nhận được những bài viết mới nhất.

Nguồn: https://namjayer.net/nhay-don-va-nhay-kep-trong-php/
